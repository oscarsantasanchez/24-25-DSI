# 📄 Informe de Análisis del Sistema de Control de Asistencia

## 1. 🧭 Resumen Ejecutivo

Este informe analiza el sistema actual de control de asistencia basado en esta [hoja de cálculo](https://docs.google.com/spreadsheets/d/1OeL1xvfuA157cCbNjkbMuJjVXL_BymwgOi7VCyGmXmE/edit?usp=sharing) para una asignatura universitaria. Se evalúan sus fortalezas, debilidades y se proponen mejoras tecnológicas e innovaciones orientadas a optimizar la gestión de datos, automatizar procesos y mitigar la inasistencia estudiantil, especialmente en días con baja participación.

---

## 2. 📝 Análisis del Sistema Actual

La hoja de cálculo implementada actualmente permite:

- Registrar la **asistencia diaria** de estudiantes.
- Calcular el **porcentaje de asistencia por alumno** (sesiones asistidas / sesiones totales).
- Mostrar:
  - Total de alumnos.
  - Número de alumnos por grados: **GII**, **GIOI**, **GADE**, **PI (Programa Internacional)**.
  - **% de asistencia diario,** general y por grado.
- Controlar el **tiempo invertido en pasar lista** cada día.
- Analizar patrones de asistencia en días específicos (**lunes vs. viernes**).

---

## 3. ⚠️ Problemática Identificada

### 3.1 Limitaciones del Sistema
- Escalabilidad reducida a una sola asignatura.
- Vulnerabilidad a errores humanos (modificación manual).
- Análisis de datos limitado y no automatizado.

### 3.2 Inasistencia Estudiantil
- Patrón de ausencias en días concretos (especialmente **viernes**).
- Potenciales causas: horarios, desmotivación, sobrecarga académica.

---

## 4. 🔧 Propuestas de Mejora y Ajustes Tecnológicos

| Categoría        | Propuesta     |
|-|-|
| Seguridad y control        | Reforzar el archivo principal con control de versiones en la nube (Google Drive) para asegurar trazabilidad y recuperación ante errores.   |
| Visualización docente      | Creación de una hoja interna con **tablas dinámicas** y **gráficos de asistencia por día/grado** solo visibles por el profesor.                    |
| Análisis de datos          | Integración con **Power BI** u otras herramientas visuales para explorar tendencias globales si se manejan varias asignaturas o grupos.             |
| Participación del alumnado | Uso de formularios anónimos para recoger **feedback cualitativo** sobre dificultades o mejoras (Google Forms).       |
| Motivación y seguimiento   | Aplicar estrategias como **mensajes recordatorio** desde la plataforma de la asignatura, e incluso dinámicas de reconocimiento a la asistencia sostenida.  |
| Mejora continua docente    | Revisión quincenal de los datos recogidos para detectar patrones de inasistencia persistente y plantear ajustes metodológicos si se considera útil. |

---

## 5. 💡 Innovaciones Sugeridas

- **Gamificación**: Recompensas o incentivos por asistencia regular.
- **Modelos predictivos**: Identificar alumnos en riesgo de abandono por baja asistencia.
- **Alertas inteligentes**: Notificaciones a estudiantes cuando bajen del 70% de asistencia.
- **Panel docente**: Visualización semanal de métricas clave.

---

## 6. 🛡️ Medidas para Mitigar la Inasistencia

| Medida  | Descripción  |
|-|-|
| Feedback semanal               | Reportes automatizados con el % de asistencia individual.                  |
| Actividades motivadoras        | Cambiar la dinámica de las sesiones del viernes.                           |
| Encuestas anónimas             | Detectar causas de inasistencia (logísticas, motivacionales, etc.).        |
| Políticas de recuperación      | Ofrecer sesiones alternativas o recuperación en línea.                     |
| Intervención temprana          | Alerta a tutoría o coordinación cuando se detecten faltas reiteradas.      |

---
## 7. 📈 Análisis Estadístico (Datos Reales)

Se han calculado métricas clave basadas en la hoja de cálculo actual:

- **Asistencia promedio global**: 78,29%
- **Estudiantes con asistencia inferior al 70%**: 17 (20,73%)
- **Asistencia media los lunes**: 60,79%
- **Asistencia media los viernes**: 78,40%
- **Grado con menor asistencia**: GADE (promedio 69%)
- **Tiempo medio en pasar lista**: 4 minutos y 27 segundos


Estas cifras refuerzan la necesidad de automatizar el proceso, implementar medidas de motivación en días críticos, e identificar a tiempo a los alumnos en riesgo de absentismo.

---

**Informe elaborado por: Óscar Santamaría**  
*Dirección de Sistemas de Información*  
*Fecha: 30/05/2025*  
