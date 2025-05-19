# Informe de Auditoría de Datos  
**Asignatura – Dirección de Sistemas de Información**  
**Archivo analizado:** `DSI-[24][25]-vAlumnos.xlsx` – 5 hojas de cálculo  
**Fecha:** 19 de mayo de 2025 (zona horaria Europe/Madrid)

---

## 1. Resumen ejecutivo

| Hoja               | Filas | Columnas | % celdas vacías | Filas duplicadas |
|--------------------|------:|---------:|---------------:|-----------------:|
| Alumnos            | 97    | 43       | **36,6 %**     | 5                |
| EC Individual      | 87    | 9        | **33,7 %**     | 0                |
| Grupos             | 113   | 20       | **48,3 %**     | 8                |
| ComponentesSI      | 92    | 10       | **14,6 %**     | 2                |
| NumerosDelParcial  | 16    | 5        | **67,5 %**     | 1                |

### Hallazgos clave

* **Estructura inconsistente:** filas‑cabecera repetidas, columnas “Unnamed” y etiquetas mezcladas con datos.  
* **Ausencia de claves primarias y relaciones explícitas** entre hojas → pérdida de trazabilidad.  
* **Valores ausentes significativos** (> 30 %) en 3 de las 5 hojas; *NumerosDelParcial* es la más crítica (~68 %).  
* **Columnas con > 50 % de valores nulos** y presencia de valores negativos donde se esperan sólo positivos.  
* **Duplicados** en *Alumnos*, *Grupos*, *ComponentesSI* y *NumerosDelParcial*.  
* **Tipos de datos heterogéneos** (texto, fechas y numéricos mezclados en las mismas columnas).

> **Impacto:** Los problemas anteriores reducen la fiabilidad analítica, encarecen las ETL y ponen en riesgo la calidad de los indicadores académicos frente a los estándares de gobierno del dato de una gran empresa.

---

## 2. Auditoría hoja a hoja

### 2.1 Alumnos
* **Contenido:** 97 filas × 43 columnas (matriz principal de estudiantes y métricas).  
* **Columnas con > 50 % nulos:** `Unnamed: 8`, `Unnamed: 9`, `0`…`0.6` (9).  
* **Anomalías:** 3 valores negativos en campos de notas/asistencia; 5 filas duplicadas.  
* **Recomendaciones:**  
  1. Definir columna **ID_Alumno** única.  
  2. Revisar fórmulas que generan valores `0.x` y columnas “Unnamed”.  
  3. Normalizar cabecera y separar métricas en tablas temáticas.

### 2.2 EC Individual
* **Contenido:** 87 filas × 9 columnas (estadísticas de examen).  
* **Problemas:** cabecera doble (filas 0‑2), columnas `-`, `-.1`, `-.2` (> 50 % nulos).  
* **Recomendaciones:** eliminar filas de título intermedias, tipar numéricos y pivotar preguntas a formato largo.

### 2.3 Grupos
* **Contenido:** 113 filas × 20 columnas (formación de grupos y entregables).  
* **Anomalías:** 8 registros duplicados; 9 columnas “Unnamed” o `max` con > 50 % nulos.  
* **Recomendaciones:**  
  * Crear clave compuesta **Grupo + Curso**.  
  * Verificar si los vacíos representan “0”.  
  * Centralizar rúbricas de evaluación en un catálogo externo.

### 2.4 ComponentesSI
* **Contenido:** 92 filas × 10 columnas (valoración de componentes SI).  
* **Calidad:** 14,6 % nulos, 2 duplicados.  
* **Recomendaciones:** etiquetar componentes y enlazarlos a estándares COBIT/ITIL.

### 2.5 NumerosDelParcial
* **Contenido:** 16 filas × 5 columnas (resumen numérico parcial).  
* **Problemas graves:** 67,5 % nulos, 1 duplicado, cabecera mal posicionada.  
* **Recomendaciones:** transponer tabla (una fila por pregunta) y depurar columnas “Unnamed”.

---

## 3. Auditoría transversal

| Métrica global                     | Valor        |
|-----------------------------------|-------------:|
| Celdas totales analizadas         | 8 214        |
| Celdas vacías                     | 3 071 (37,4 %) |
| Columnas con > 50 % vacíos        | **24**       |
| Filas duplicadas en total         | **16**       |
| Hojas con valores negativos       | **Alumnos**  |

### Consistencia inter‑hojas
* **Sin claves naturales coincidentes** (ID de alumno, grupo, etc.).  
* **Falta diccionario de datos** que defina rangos, tipos y dependencias.  
* Columnas “Unnamed” impiden trazabilidad al migrar a BBDD relacionales.

---

## 4. Recomendaciones generales

1. **Modelo de datos**  
   * Diseñar esquema estrella: tablas dimensión (`Alumnos`, `Grupos`, `ComponentesSI`) y tabla de hechos (`Resultados_Evaluación`).  
   * Definir **PK** y **FK** explícitas.

2. **Calidad y limpieza**  
   * Eliminar columnas con > 50 % vacíos o justificar su mantenimiento.  
   * Corregir valores negativos tras validar con la fuente original.  
   * Automatizar control de duplicados (Power Query / scripts ETL).

3. **Gobierno del dato**  
   * Crear diccionario de datos con definición, tipo y rango esperado.  
   * Versionar ficheros en Git con CI que valide esquema antes de *merge*.

4. **Visualización y reporting**  
   * Publicar dashboards (Power BI / Metabase) con KPI de asistencia y notas.  
   * Documentar en el README la procedencia y transformación de cada tabla.

5. **Próximos pasos**  
   * Reunión con responsables académicos para confirmar reglas de negocio.  
   * Implementar pruebas unitarias que bloqueen la carga de datos corruptos.  
   * Plan de remediación prioritario: **Grupos → Alumnos → EC Individual → NumerosDelParcial**.

---

## 5. Riesgos si no se actúa

| Riesgo                                               | Impacto | Probabilidad |
|------------------------------------------------------|--------:|-------------:|
| Informes erróneos a la dirección de la empresa       | Alto    | Alto         |
| Decisiones académicas basadas en datos incompletos   | Medio‑Alto | Medio      |
| Incremento del esfuerzo en futuras integraciones     | Alto    | Alto         |
| Pérdida de confianza de *stakeholders*               | Alto    | Medio        |

---

## 6. Conclusión
La auditoría evidencia carencias estructurales y de calidad que comprometen la fiabilidad de los análisis en **Dirección de Sistemas de Información**. Se recomienda iniciar de inmediato un plan de saneamiento y adoptar buenas prácticas de gobierno del dato para alinear el repositorio con los estándares de una gran empresa.

> *“Lo que no se mide no se puede mejorar; lo que se mide mal, se empeora.”* – Adaptación de Lord Kelvin
