---
marp: true
theme: default
backgroundColor: #fff
paginate: true
_paginate: false
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---

<style>
section {
  font-size: 30px;
}
h1 {
  color: #0366d6;
}
h2 {
  color: #0366d6;
}
.columns {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1rem;
}
.columns-3 {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1rem;
}
table {
  font-size: 24px;
}
.code-block {
  background-color: #f6f8fa;
  padding: 1rem;
  border-radius: 8px;
  font-family: monospace;
}
.highlight {
  color: #d73a49;
  font-weight: bold;
}
.impact {
  font-size: 34px;
  color: #0366d6;
  text-align: center;
  margin: 1rem 0;
}
</style>

# Operaciones y Servicios (Parte 2)
### Enfoques modernos y gestión continua

---

## Contexto: Lo que hemos visto

<div class="columns">
<div>

### ITSM + ITIL
- Gestión de servicios estructurada
- Procesos estandarizados
- Impacto empresarial 

</div>
<div>

### Infraestructura
- Tipos de servidores y su administración  
- Computación en la nube
- Modelos financieros (CAPEX vs OPEX)

</div>
</div>

**Ahora**: Veremos enfoques modernos que aumentan la agilidad y eficiencia operativa

---

1. **DevOps y Site Reliability Engineering (SRE)**
2. **Automatización operativa**
3. **Observabilidad y monitorización**
4. **Medición y mejora de servicios**
5. **Continuidad y recuperación**
6. **Aplicación práctica según sector**

---

# DevOps & SRE

## La evolución de las operaciones

![bg right:35% 80%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Devops-toolchain.svg/1200px-Devops-toolchain.svg.png)

---

## El problema de la separación tradicional

<div class="columns">
<div>

### Desarrolladores
- **Objetivo**: Entregar nuevas funciones
- **Métrica principal**: Velocidad de entrega
- **Prioridad**: Cambio e innovación

</div>
<div>

### Operaciones
- **Objetivo**: Mantener estabilidad
- **Métrica principal**: Disponibilidad
- **Prioridad**: Control y seguridad

</div>
</div>

**Resultado real**: Retrasos, conflictos y servicios deficientes para el negocio

---

## DevOps: Principios fundamentales

1. **Cultura de colaboración**: Equipos integrados en lugar de separados
2. **Automatización**: Reducir tareas manuales y repetitivas
3. **Medición constante**: Decisiones basadas en datos reales
4. **Mejora continua**: Aprender y ajustar constantemente
5. **Responsabilidad compartida**: "Si lo construyes, lo operas"

<div class="impact">
"Las empresas con DevOps avanzado despliegan 
cambios 200 veces más rápido" - State of DevOps Report
</div>

---

## DevOps en diferentes sectores

<div class="columns">
<div>

### Tecnología
- Entregas diarias o continuas
- Equipos multifuncionales
- Ejemplo: Spotify, Amazon

</div>
<div>

### Industria
- Integración de software en maquinaria
- Monitorización predictiva
- Ejemplo: Smart factories, IoT industrial

</div>
</div>

---

## Site Reliability Engineering (SRE)

### La visión de Google sobre operaciones

Aplicar ingeniería de software a los problemas de operaciones.

<div class="columns">
<div>

### Principios SRE
- Presupuesto de error: cuánto puede fallar un sistema
- Eliminar tareas operativas repetitivas
- Automatización por defecto
- Degradación gradual en lugar de fallos completos

</div>
<div>

### Métricas clave simplificadas
- **SLO**: Objetivo de nivel de servicio (ej: 99.9% disponible)
- **SLI**: Indicador real medido (ej: % de peticiones exitosas)
- **Error budget**: Margen permitido de fallos (ej: 0.1% del tiempo)

</div>
</div>

---

## Comparativa de enfoques

|Característica|Enfoque tradicional|DevOps|SRE|
|-|-|-|-|
|**Cambios**|Grandes y arriesgados|Pequeños y frecuentes|Basados en presupuesto de error|
|**Equipos**|Separados|Colaborativos|Integrados|
|**Prioridad**|Estabilidad o velocidad|Balance y automatización|Confiabilidad y escala|
|**Aplicación**|Cualquier empresa|Organizaciones ágiles|Entornos de gran escala|

---

## Las 4 señales doradas de SRE

<div class="columns-3">
<div>

### Latencia
Tiempo de respuesta  
"¿Cuánto tarda?"

</div>
<div>

### Tráfico  
Volumen de demanda
"¿Cuántas peticiones?"

</div>
<div>

### Errores
Tasa de fallos
"¿Cuánto falla?"

</div>
</div>

### Saturación
Nivel de uso de recursos (CPU, memoria, red)
"¿Cuánta capacidad queda?"

---

# Automatización Operativa

## Reduciendo el trabajo manual repetitivo

![bg right:35% 80%](https://images.unsplash.com/photo-1495317987375-ce0780d0a1ab)

---

## ¿Por qué automatizar? El caso de negocio

<div class="columns">
<div>

### Problemas del trabajo manual
- Error humano: causa del 70% de los fallos
- Inconsistencia entre entornos
- Imposible escalar con personas
- Conocimiento en silos (dependencia de expertos)

</div>
<div>

### Beneficios cuantificables  
- Reducción de errores: hasta 90%
- Tiempo de respuesta: de horas a minutos
- Aumento de capacidad sin personal adicional
- ROI típico: 3-6 meses

</div>
</div>

---

## Automatización progresiva

|Nivel|Qué se automatiza|Beneficio empresarial|Ejemplo concreto|
|-|-|-|-|
|**Básico**|Tareas individuales|Ahorro de tiempo puntual|Script de copia de seguridad diaria|
|**Intermedio**|Procesos completos|Consistencia y velocidad|Despliegue completo de servidores web|
|**Avanzado**|Infraestructura completa|Agilidad organizacional|Entorno completo creado en minutos|
|**Inteligente**|Auto-reparación|Reducción drástica de incidentes|Sistema que se recupera solo de fallos|

---

## Infraestructura como Código (simplificado)

<div class="columns">
<div>

### Concepto básico
Describir la infraestructura en archivos de texto que pueden:
- Guardarse en control de versiones
- Revisarse como código normal
- Ejecutarse automáticamente
- Reproducirse exactamente igual

</div>
<div>

### Analogía
Es como tener la "receta" exacta para crear:
- Servidores
- Redes
- Bases de datos
- Entornos completos

</div>
</div>

---

## Despliegue continuo (CI/CD)

<div class="columns">
<div>

### Proceso manual tradicional
1. Desarrollo (semanas/meses)
2. Pruebas separadas (días/semanas)
3. Preparación (días)
4. Despliegue con riesgo (horas/días)

**Total**: Semanas o meses

</div>
<div>

### Proceso automatizado
1. Desarrollo iterativo
2. Pruebas automáticas inmediatas
3. Verificación automática
4. Despliegue automatizado

**Total**: Minutos u horas

</div>
</div>

---

## Ejemplos de automatización por sector

<div class="columns-3">
<div>

### TI
- Despliegue de aplicaciones
- Gestión de configuración
- Copias de seguridad

</div>
<div>

### Industria
- Control de calidad
- Mantenimiento predictivo
- Gestión de inventario

</div>
<div>

### Empresarial
- Procesos financieros
- Análisis de datos
- Servicio al cliente

</div>
</div>

---

# Observabilidad

## Entendiendo sistemas complejos

![bg right:35% 80%](https://images.unsplash.com/photo-1551288049-bebda4e38f71)

---

## Evolución de la supervisión

<div class="columns">
<div>

### Monitorización tradicional
- Comprueba si algo funciona o no
- Alertas basadas en umbrales fijos
- Enfoque reactivo (avisa cuando falla)
- Limitado a lo que se configuró previamente

</div>
<div>

### Observabilidad moderna
- Permite entender por qué algo no funciona
- Análisis flexible de problemas desconocidos
- Enfoque proactivo (detecta antes de fallar)
- Adaptable a situaciones no previstas

</div>
</div>

---

## Los tres elementos esenciales

<div class="columns-3">
<div>

### Métricas
Valores numéricos medidos
continuamente

**Ejemplo**: Uso CPU = 75%

</div>
<div>

### Registros (logs)
Eventos detallados con  
información de contexto

**Ejemplo**: Error al procesar ID 12345 a las 15:30

</div>
<div>

### Trazas
Seguimiento de operaciones
a través de múltiples sistemas

**Ejemplo**: Recorrido de un pedido desde la web hasta el almacén

</div>
</div>

---

## Observabilidad en acción: Caso práctico

<div class="columns">
<div>

### Escenario: Lentitud en aplicación comercial
**Enfoque tradicional**:
- Verificar si los servidores funcionan
- Comprobar uso de recursos
- Reiniciar sistemas
- Horas o días hasta resolver

</div>
<div>

### Con observabilidad moderna
- Identificar transacciones lentas exactas
- Ver recorrido completo del proceso
- Localizar componente específico con problema
- Resolución en minutos

</div>
</div>

---

# Medición y Mejora

## Gestión basada en datos reales

![bg right:35% 80%](https://images.unsplash.com/photo-1460925895917-afdab827c52f)

---

## Presupuesto de error: Equilibrando estabilidad e innovación

<div class="columns">
<div>

### Concepto en lenguaje simple
Si nuestro objetivo es 99.9% disponibilidad:
- Tenemos 0.1% "permitido" para fallos
- = 43.8 minutos/mes
- Mientras no superemos ese límite, podemos seguir innovando

</div>
<div>

### Beneficios para la organización
- Balance entre innovar y estabilizar
- Decisiones objetivas sobre riesgos
- Reduce conflictos entre áreas
- Priorización basada en datos

</div>
</div>

---

## Indicadores clave para servicios modernos

|Métrica|Explicación sencilla|Impacto en el negocio|
|-|-|-|
|**MTTD**|Tiempo en detectar problemas|Menos tiempo = menor impacto|
|**MTTR**|Tiempo en recuperar el servicio|Mide velocidad de respuesta a incidentes|
|**Deployment frequency**|Frecuencia de cambios|Mayor = más agilidad|
|**Change failure rate**|% de cambios que causan problemas|Menor = más calidad|

---

## Comparativa de rendimiento en la industria

<div class="columns">
<div>

### Bajo rendimiento
- Despliegues: 1 por mes
- MTTR: Días o semanas
- Tasa de fallos: >45%
- Tiempo para cambios: 6+ meses

</div>
<div>

### Alto rendimiento
- Despliegues: Múltiples por día
- MTTR: Menos de 1 hora
- Tasa de fallos: <5%
- Tiempo para cambios: Menos de 1 día

</div>
</div>

<div class="impact">
Las organizaciones de alto rendimiento son 2.5 veces más probables 
de superar sus objetivos comerciales
</div>

---

## Análisis de causa raíz: Método de los 5 Porqués

**Ejemplo práctico: Sistema de facturación fallando**

<div class="columns">
<div>

### Problema superficial
1. ¿Por qué? El sistema está lento
2. ¿Por qué? Base de datos sobrecargada
3. ¿Por qué? Consultas ineficientes
4. ¿Por qué? No se revisó el rendimiento
5. ¿Por qué? No hay proceso de revisión

</div>
<div>

### Solución real
- Superficial: Reiniciar sistema
- Profunda: Implementar proceso de revisión de rendimiento antes de cada despliegue

**Impacto**: Prevención de futuros problemas

</div>
</div>

---

# Continuidad y Recuperación

## Preparación para interrupciones

![bg right:35% 80%](https://images.unsplash.com/photo-1558494949-ef010cbdcc31)

---

## Los dos parámetros críticos

<div class="columns">
<div>

### RPO (Recovery Point Objective)
- **Pregunta**: ¿Cuántos datos podemos permitirnos perder?
- **Ejemplo**: RPO = 1 hora significa perder como máximo 1 hora de datos
- **Impacto financiero**: Mayor = más barato pero más pérdida potencial

</div>
<div>

### RTO (Recovery Time Objective)
- **Pregunta**: ¿Cuánto tiempo podemos estar sin servicio?
- **Ejemplo**: RTO = 4 horas significa volver a funcionar en máximo 4 horas
- **Impacto financiero**: Menor = más costoso pero menos pérdidas por caída

</div>
</div>

---

## Estrategias de recuperación para cada necesidad

|Estrategia|Explicación sencilla|Coste relativo|Tipos de servicios|
|-|-|-|-|
|**Backup y restauración**|Copias de seguridad periódicas|€|Datos no críticos|
|**Backup en caliente**|Copias en tiempo real o casi real|€€|Sistemas importantes|
|**Sistemas redundantes**|Duplicación de componentes críticos|€€€|Servicios críticos|
|**Multi-región/zona**|Sistemas en múltiples ubicaciones físicas|€€€€|Servicios esenciales|

---

## Plan de recuperación ante desastres:<br> componentes esenciales

1. **Análisis de impacto en el negocio**: Cuantificar el costo de las interrupciones
2. **Inventario de sistemas críticos**: Priorizar qué recuperar primero
3. **Procedimientos documentados**: Pasos exactos a seguir
4. **Roles y responsabilidades**: Quién hace qué durante la crisis
5. **Pruebas regulares**: Verificar que el plan realmente funciona

<div class="impact">
"40% de las empresas que sufren un desastre sin plan 
no vuelven a abrir." - Gartner
</div>

---

## Continuidad por sector: ejemplos prácticos

<div class="columns-3">
<div>

### TI
- Sistemas redundantes
- Centros de datos alternativos
- Replicación de datos

</div>
<div>

### Industria
- Sistemas de respaldo para control
- Procedimientos manuales alternativos
- Inventarios de seguridad

</div>
<div>

### Servicios financieros
- Centros de operaciones alternativos
- Replicación en tiempo real
- Pruebas trimestrales obligatorias

</div>
</div>

---

# Aplicación práctica por sector

## Adaptación a diferentes necesidades

---

## Tecnologías de la Información

<div class="columns">
<div>

### Desafíos específicos
- Ritmo acelerado de cambio tecnológico
- Expectativas de disponibilidad 24/7
- Seguridad y cumplimiento normativo
- Escalabilidad variable

</div>
<div>

### Enfoque recomendado
- CI/CD + infraestructura como código
- SRE para servicios críticos
- Observabilidad multinivel
- Automatización extensiva

</div>
</div>

---

## Entornos Industriales

<div class="columns">
<div>

### Desafíos específicos
- Integración IT/OT (Tecnología operativa)
- Restricciones de seguridad física
- Impacto directo en producción
- Ciclos de vida más largos

</div>
<div>

### Enfoque recomendado
- Automatización gradual y validada
- Monitorización predictiva
- Planes de continuidad robustos
- Gestión del cambio controlada

</div>
</div>

---

## Servicios empresariales

<div class="columns">
<div>

### Desafíos específicos
- Orientación a procesos de negocio
- Cumplimiento regulatorio
- Variabilidad estacional
- Experiencia del cliente

</div>
<div>

### Enfoque recomendado
- Observabilidad centrada en KPIs de negocio
- Automatización de procesos (RPA)
- Análisis de impacto empresarial
- Gestión por métricas comerciales

</div>
</div>

---

# Tendencias y futuro

## Evolución de las operaciones

---

## AIOps: Inteligencia artificial en operaciones

<div class="columns">
<div>

### Capacidades principales
- Detección automática de anomalías
- Predicción de problemas futuros
- Correlación inteligente de eventos
- Recomendaciones de resolución

</div>
<div>

### Beneficios empresariales
- Reducción del 50% en incidentes no detectados
- Diagnóstico un 60% más rápido
- Automatización de respuestas de primer nivel
- Mejora continua basada en patrones

</div>
</div>

---

## Optimización de costos en la nube (FinOps)

<div class="columns">
<div>

### El problema
- Costos cloud no controlados
- Aumento del 30-45% anual en gasto
- Recursos aprovisionados en exceso
- Falta de visibilidad del consumo

</div>
<div>

### Soluciones prácticas
- Asignación y monitorización por departamento
- Instancias reservadas (ahorro 30-60%)
- Apagado automático de recursos no utilizados
- Rightsizing (ajuste de recursos a necesidad real)

</div>
</div>

---

# Conclusiones

## Puntos clave de la evolución operativa

---

## 1. Transformación de mentalidad

<div class="columns">
<div>

### De procesos a cultura
- ITIL como marco útil no como dogma
- DevOps como cultura de colaboración
- SRE como ingeniería de confiabilidad
- Datos como base de decisiones

</div>
<div>

### Beneficios reales
- Mayor velocidad de innovación
- Menos conflictos interdepartamentales
- Mejora en satisfacción de clientes
- Eficiencia operativa mejorada

</div>
</div>

---

## 2. Automatización inteligente

<div class="impact">
"No es automatizar por automatizar, es eliminar el trabajo 
repetitivo para centrarse en lo que aporta valor"
</div>

- Infraestructura como código = Consistencia y velocidad
- Observabilidad = Comprensión profunda de sistemas
- Auto-reparación = Reducción drástica de incidentes
- Medición = Base para la mejora continua

---

## 3. La ecuación ganadora

|||
|-|-|
Marco de procesos (ITIL)|+ 
Cultura colaborativa (DevOps)|+ 
Ingeniería de confiabilidad (SRE)|+ 
Automatización inteligente|+ 
Infraestructura flexible (Cloud)|= 
**Operaciones que impulsan el negocio en vez de frenarlo**


---

## 4. Competencias del futuro

<div class="columns-3">
<div>

### Técnicas
- Automatización
- Cloud multiplataforma
- Observabilidad
- Seguridad integrada

</div>
<div>

### Personas
- Colaboración efectiva
- Visión de conjunto
- Adaptabilidad
- Comunicación clara

</div>
<div>

### Negocio
- Análisis de valor
- Orientación a resultados
- Mejora continua
- Gestión del cambio

</div>
</div>

---

# Plan de acción

## Pasos concretos para avanzar

---

## Fase 1: Fundamentos (3-6 meses)

1. Adoptar ITIL para estructura básica y terminología común
2. Implementar monitorización centralizada con alertas útiles
3. Documentar procesos críticos y crear playbooks de respuesta
4. Identificar tareas manuales repetitivas para automatizar

---

## Fase 2: Evolución (6-12 meses)

1. Introducir prácticas DevOps en áreas seleccionadas
2. Crear plataforma básica de automatización de despliegues
3. Implementar observabilidad para servicios críticos
4. Definir SLAs, SLOs y error budgets para servicios principales

---

## Fase 3: Transformación (12-24 meses)

1. Adoptar infraestructura como código
2. Implementar CI/CD completo para aplicaciones clave
3. Establecer equipos con enfoque SRE
4. Desarrollar medición integral de resultados de negocio

---

# Recursos para continuar

- [SRE Book - Google](https://sre.google/sre-book/) - Fundamentos de SRE
- [State of DevOps Report](https://cloud.google.com/devops/state-of-devops/) - Benchmarks de la industria
- [Cloud Adoption Framework](https://azure.microsoft.com/en-us/cloud-adoption-framework/) - Migración a cloud
- [FinOps Foundation](https://www.finops.org/) - Optimización de costos cloud
- [DORA Metrics](https://www.devops-research.com/research.html) - Medición de rendimiento

---

# Reflexión final

Las operaciones modernas no son un centro de coste,
sino un elemento estratégico que potencia la capacidad 
de la organización para innovar, adaptarse y crecer.