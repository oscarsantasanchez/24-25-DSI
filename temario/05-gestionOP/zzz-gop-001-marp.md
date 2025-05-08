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

# Operaciones y servicios<br>de Sistemas de Información

## Gestión y mantenimiento de servicios de TI

---

1. **Introducción**: ¿Por qué son importantes las operaciones?
2. **Fundamentos de la gestión de servicios**
   - Gestión de Servicios de TI (ITSM)
   - Marco ITIL
3. **Infraestructura tecnológica**
   - Servidores y administración
   - Computación en la nube
4. **Casos prácticos y aplicación transversal**

---

## ¿Por qué?

![bg right:35% 80%](https://images.unsplash.com/photo-1550751827-4bd374c3f58b?w=800)

La mejor estrategia y el proyecto mejor ejecutado **fracasan** sin una operación adecuada que mantenga los sistemas funcionando correctamente día a día.

<div class="impact">
"Un minuto de caída puede costar a una empresa de comercio electrónico €5.000-€10.000 en ventas perdidas."
</div>

---

## El desafío operativo: impacto real

<div class="columns">
<div>

### Complejidad creciente

- Entornos locales
- Servicios cloud
- Aplicaciones de terceros  
- Desarrollos propios

</div>
<div>

### Impacto cuantificable

- **Financiero**: €5.000-€100.000/hora según sector
- **Productividad**: 50-100% pérdida en empleados
- **Reputación**: 30% clientes no regresa tras fallo
- **Regulatorio**: Multas por incumplimiento

</div>
</div>

---

## Ejemplos del mundo real

<div class="columns">
<div>

### Servicios digitales
**Outage de AWS (2021)**
- 7 horas de interrupción
- Afectó a Netflix, Disney+, Venmo
- Pérdidas estimadas: $150M

</div>
<div>

### Producción industrial
**Fallo en sistema MES**
- Línea de producción parada 4 horas
- 240 vehículos no fabricados
- Impacto: €2.4M + retrasos en cadena

</div>
</div>

---

# [Apagón en la península ibérica de 2025](https://es.wikipedia.org/wiki/Apag%C3%B3n_en_la_pen%C3%ADnsula_ib%C3%A9rica_de_2025)

---

## ITSM en contextos diversos

<div class="columns">
<div>

### Tecnología
- Sistemas corporativos
- Aplicaciones empresariales
- Infraestructura TI

</div>
<div>

### Más allá de TI
- **Industria**: Monitorización de equipos, mantenimiento predictivo
- **Logística**: Seguimiento de pedidos, gestión de rutas
- **Finanzas**: Procesamiento de transacciones, cumplimiento normativo

</div>
</div>

---

## ¿Qué son las operaciones de TI?

> Conjunto de trabajos y métodos para que los servicios tecnológicos funcionen ***sin interrupciones, con calidad y mejoren con el tiempo***.

<div class="columns-3">
<div>

### Gestión de servicios
- Procesos organizados
- Acuerdos de nivel
- Resolución de problemas

</div>
<div>

### Infraestructura  
- Equipos físicos
- Redes
- Recursos cloud

</div>
<div>

### Entrega continua
- Supervisión
- Automatización
- Disponibilidad

</div>
</div>

---

## El ciclo PODC en operaciones

|Fase|Actividades|Ejemplo concreto|
|-|-|-|
|**Planificar**|Diseño de servicios, Capacidad|Plan de capacidad para campaña de ventas Black Friday|
|**Organizar**|Implementación, Configuración|Preparación de servidores y recursos antes del evento|
|**Dirigir**|Operación diaria, Incidentes|Supervisión durante el evento y gestión de problemas|
|**Controlar**|Monitorización, Mejora|Análisis post-evento y mejoras para el siguiente año|

---

# Fundamentos: ITSM

## Information Technology Service Management

![bg right:30% 90%](https://blog.invgate.com/hs-fs/hubfs/inf-fundaciones-itil.png?width=1616&name=inf-fundaciones-itil.png)

---

## ¿Por qué ITSM?

<div class="columns">
<div>

### Dependencia crítica de TI
- Procesos que dependen 100% de la tecnología
- Equipos industriales conectados
- Transacciones financieras automatizadas
- Servicios públicos digitalizados

</div>
<div>

### Complejidad organizacional
- Sistemas heredados
- Soluciones actuales  
- Tecnologías emergentes
- Integración entre diferentes áreas

</div>
</div>

---

## Elementos fundamentales ITSM

|Elemento|Descripción|Ejemplos en diferentes sectores|
|-|-|-|
|**Servicios**|Entregar valor sin que los usuarios asuman riesgos|TI: Email corporativo<br>Industrial: Sistema de control de calidad<br>ADE: CRM|
|**Procesos**|Actividades estructuradas con entradas/salidas|TI: Gestión de cambios<br>Industrial: Mantenimiento preventivo<br>ADE: Aprobación de gastos|
|**SLAs**|Compromisos de calidad y disponibilidad|*99.9% disponibilidad* = máximo 8h 45m caída/año|

---

![bg fit center:40%](https://www.servicetonic.com/wp-content/uploads/2016/12/ejemplo-de-un-buen-SLA.png)

---

## Ejemplo de SLA en diferentes contextos

- **TI**: 99.9% disponibilidad del correo
- **Industrial**: Tiempo de respuesta < 1h para averías críticas
- **Comercial**: Resolución < 24h para incidencias de clientes VIP

---

## Áreas clave de ITSM

<div class="columns">
<div>

### Reactivas
- Gestión de incidentes
- Resolución de problemas  
- Restauración de servicios

**Ejemplo**: *Cuando un sistema de facturación falla, ¿cómo restaurarlo rápidamente?*

</div>
<div>

### Proactivas  
- Gestión de cambios
- Gestión de la capacidad
- Gestión de la disponibilidad

**Ejemplo**: *¿Cómo asegurar que el sistema soportará el volumen de la campaña de Navidad?*

</div>
</div>

---

# Marco ITIL

## Information Technology Infrastructure Library

![bg right:35% 80%](https://www.owlpoint.com/wp-content/uploads/2019/08/The-4-Dimensions-of-Managment-m.jpg)

---

## Evolución de ITIL

|Versión|Año|Enfoque|Contexto histórico|
|-|-|-|-|
|**ITIL v1**|1989-1995|Operaciones de TI|Inicios de TI corporativa estructurada|
|**ITIL v2**|2000-2006|Procesos de servicio|Era de internet y expansión de TI|
|**ITIL v3**|2007-2011|Ciclo de vida del servicio|Digitalización y servicios móviles|
|**ITIL 4**|2019-presente|Valor y transformación digital|Cloud, IA, automatización|

---

## ITIL 4: Sistema de valor simplificado

<div class="columns">
<div>

### Principios guía
1. Enfocarse en el valor
2. Comenzar donde estás
3. Mejorar paso a paso
4. Trabajar colaborativamente
5. Visión completa del sistema

</div>
<div>

### Cadena de valor esencial
- Planificar lo que se necesita
- Diseñar soluciones adecuadas
- Construir servicios de calidad
- Entregar de forma confiable
- Mejorar constantemente

</div>
</div>

---

## Prácticas clave de ITIL 4

<div class="columns-3">
<div>

### Gestión general
- Estrategia
- Seguridad
- Finanzas

</div>
<div>

### Gestión de servicios
- Mesa de ayuda
- Gestión de incidentes
- Gestión de problemas
- Gestión de cambios

</div>
<div>

### Gestión técnica  
- Infraestructura
- Arquitectura
- Operaciones

</div>
</div>

---

# Infraestructura Tecnológica

## La base de todo servicio digital

![bg right:35% 90%](https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=800)

---

## ¿Por qué infraestructura?

<div class="columns">
<div>

### Base tecnológica sólida
- Recursos centralizados
- Procesos críticos
- Especialización funcional

</div>
<div>

### Eficiencia y escalabilidad
- Adaptación a la demanda
- Optimización costos
- Seguridad y control

</div>
</div>

---

## Componentes de infraestructura

|Componente|Descripción|Ejemplos cotidianos|
|-|-|-|
|**Hardware**|Equipos físicos|Servidores, ordenadores, dispositivos móviles|
|**Software base**|Control de recursos|Windows/Linux, bases de datos, navegadores|
|**Redes**|Comunicación de datos|WiFi, Internet, intranet corporativa|
|**Instalaciones**|Espacios físicos|Centros de datos, salas de servidores|

---

## Modelos de infraestructura

<div class="columns">
<div>

### Tradicional (On-premise)
- Se compra e instala todo
- Inversión grande inicial
- Control total
- Ciclos de renovación cada 3-5 años

</div>
<div>

### Cloud (En la nube)
- Se alquila según se necesita
- Pago mensual por lo que se usa
- Flexibilidad para crecer o reducir
- Siempre actualizado

</div>
</div>

---

## Tendencias en infraestructura

1. **Virtualización** → Usar un servidor físico como si fueran muchos
2. **Automación** → Configurar sistemas mediante programación
3. **Edge Computing** → Procesamiento cerca del usuario final
4. **Sostenibilidad** → Reducir consumo energético
5. **IA aplicada** → Sistemas que se autogestionan

---

# Servidores

## El corazón de la infraestructura

![bg right:40% 90%](https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=800)

---

## Tipos de servidores simplificados

<div class="columns">
<div>

### Por implementación
- Físicos dedicados (equipos reales)
- Virtualizados (compartiendo hardware)
- En la nube (alquilados)

</div>
<div>

### Por función
- Web (sitios y aplicaciones)
- Bases de datos (almacén de información)
- Aplicaciones (lógica de negocio)
- Archivos (documentos compartidos)

</div>
</div>

---

## Ciclo de administración

|Fase|Actividades|Ejemplo práctico|
|-|-|-|
|**Planificación**|Requisitos, diseño, dimensionamiento|Calcular recursos necesarios para el ERP|
|**Implementación**|Instalación, configuración, pruebas|Poner en marcha los servidores necesarios|
|**Operación**|Supervisión, mantenimiento, parches|Mantener funcionando día a día|
|**Optimización**|Rendimiento, capacidad, actualizaciones|Mejorar velocidad y añadir memoria|
|**Retirada**|Migración, backup, desmantelamiento|Sustituir por un sistema nuevo|

---

## Gestión de servidores: desafíos comunes

<div class="columns">
<div>

### Proliferación
- Demasiados servidores difíciles de gestionar
- "Un servidor para cada cosa" causa ineficiencia

</div>
<div>

### Actualizaciones
- Equilibrar seguridad vs. estabilidad
- Ventanas de mantenimiento limitadas

</div>
</div>

<div class="columns">
<div>

### Supervisión
- Distinguir problemas reales de falsos positivos
- Recopilar información útil sin sobrecarga

</div>
<div>

### Seguridad
- Protección contra amenazas
- Control de quién accede y qué puede hacer

</div>
</div>

---

# Computación en la Nube

## Transformando la infraestructura

![bg right:35% 90%](https://cdn-icons-png.flaticon.com/512/4215/4215831.png)

---

## Cloud: comparativa de modelos

<div class="columns">
<div>

### Modelo tradicional
- Gran inversión inicial (CAPEX)
- Ciclos de compra de 3-5 años
- Capacidad fija difícil de cambiar
- Mantenimiento propio

</div>
<div>

### Modelo cloud
- Gasto operativo mensual (OPEX)
- Flexibilidad inmediata
- Capacidad ajustable según necesidad
- Mantenimiento incluido

</div>
</div>

---

## Características de cloud explicadas

|Característica|Descripción|Ejemplo cotidiano|
|-|-|-|
|**Autoservicio bajo demanda**|Obtener recursos cuando se necesitan|Como elegir una película en Netflix|
|**Acceso amplio**|Disponible desde cualquier dispositivo|Como el correo electrónico personal|
|**Recursos compartidos**|Infraestructura usada por muchos clientes|Como un edificio de apartamentos|
|**Elasticidad rápida**|Ampliar o reducir según necesidad|Como la luz: pagas lo que consumes|
|**Servicio medido**|Facturación por uso real|Como la factura del teléfono móvil|

---

## Modelos de servicio simplificados

|Modelo|Concepto|Ejemplo concreto|Como si fuera...|
|-|-|-|-|
|**SaaS**|Software como servicio|Office 365, Salesforce|Restaurante: solo comes|
|**PaaS**|Plataforma como servicio|Google App Engine|Cocina preparada: tú cocinas|
|**IaaS**|Infraestructura como servicio|AWS EC2, Azure VMs|Alquiler casa: tú la equipas|

---

## Cloud: beneficios económicos cuantificables

<div class="columns">
<div>

### Ventajas financieras
- Reducción de inversión inicial: 100% → 0%
- Conversión CAPEX → OPEX
- TCO: Reducción del 30-50% en 5 años
- Ejemplo: Servidor €10.000 vs €200/mes

</div>
<div>

### Ventajas operativas  
- Tiempo de despliegue: semanas → minutos
- Escalado automático en picos de demanda
- Disponibilidad típica: 99.9-99.99%
- Acceso global instantáneo

</div>
</div>

<sub>*CAPEX: Gastos de capital / OPEX: Gastos operativos / TCO: Coste de propiedad*</sub>

---

## Cloud: Modelo de costos comparado

<div class="columns">
<div>

### On-premise (5 años)
- Hardware: €50.000
- Software: €30.000
- Mantenimiento: €40.000
- Electricidad: €15.000
- Personal: €125.000
- **Total: €260.000**

</div>
<div>

### Cloud (5 años)
- Servicios IaaS/PaaS: €90.000
- Gestión: €40.000
- Personal: €70.000
- **Total: €200.000**
- **Ahorro: 23%**
- **Beneficio adicional: flexibilidad**

</div>
</div>

<sub>*On-premise: en las instanaciones*</sub>

---

## Cloud: Adopción estratégica

### Enfoques prácticos
1. **Lift & Shift**: Mover como está → Rápido pero menos eficiente
2. **Replatform**: Ajustes moderados → Balance esfuerzo/beneficio  
3. **Refactor**: Rediseño completo → Máximo beneficio pero costoso
4. **Replace**: Usar alternativa SaaS → Lo más simple cuando existe

---

# Casos de estudio

## Operaciones en acción

---

## Caso 1: Incidente crítico en banca

**Situación**: Caída del servidor de base de datos que afecta a cajeros automáticos

**Impacto empresarial**:
- 2.500 transacciones/hora no procesadas
- Pérdida de €15.000/hora en comisiones
- Daño reputacional cuantificable

**Respuesta ITSM**:
- Activación de protocolo de crisis (15 min)
- Failover a sistema secundario (30 min)
- Resolución completa y análisis posterior (4h)

---

## Caso 2: Migración a cloud en retail

**Escenario**: Cadena de tiendas migra su sistema de inventario a AWS

**Análisis financiero**:
- Inversión en migración: €120.000
- Ahorro anual: €80.000
- ROI: 1,5 años

**Resultados operativos**:
- Tiempo de implementación: 4 meses vs 9 meses tradicional
- Reducción de fallos de inventario: 35%
- Aumento de velocidad en aperturas de tiendas: 60%

---

# Integración de conceptos

## Conectando los puntos

---

## ITSM + Infraestructura: Impacto real

<div class="columns">
<div>

### Antes
- Gestión reactiva: resolver cuando falla
- Procesos manuales propensos a errores
- Infraestructura fija con capacidad estimada

</div>
<div>

### Ahora
- Prevención y automatización
- Procesos repetibles y auditables
- Infraestructura que se adapta a la demanda

**Resultado**: 70% menos incidentes, 40% reducción en tiempo de respuesta

</div>
</div>

---

## Aplicación transversal

```
ITSM aplicado en diferentes contextos:

• TI: Gestión centralizada de servicios digitales
• Industria: Mantenimiento predictivo, monitorización de producción
• ADE: Entrega consistente de servicios al cliente, análisis de datos
• Común: Mejora de calidad, reducción de costos, experiencia del usuario
```

---

# Conclusiones

## Puntos clave

---

## 1. Evolución operativa

**De**: Gestión reactiva y manual de problemas  
**A**: Enfoque proactivo, organizado y escalable

**Valor empresarial**: 
- Reducción de costos operativos (25-40%)
- Mayor satisfacción de usuarios y clientes

---

## 2. Infraestructura moderna

**Combinación ideal**:
- Procesos ITSM bien definidos
- Infraestructura flexible y escalable  
- Medición constante y mejora

**ROI típico**: 30-40% en 3 años

---

## 3. Futuro híbrido y flexible

<div class="columns">
<div>

### Estrategia integrada
- Combinar on-premise y cloud según necesidad
- Procesos adaptativos al entorno
- Medición alineada con objetivos de negocio

</div>
<div>

### Competencias necesarias
- Gestión de servicios
- Conocimientos técnicos aplicados
- Visión de procesos de negocio
- Análisis financiero de TI

</div>
</div>

---

# Recursos adicionales

- [ITIL 4 Foundation](https://www.axelos.com/certifications/itil-certifications/itil-foundation)
- [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected/)
- [Google SRE Book](https://sre.google/sre-book/table-of-contents/)
- [Medición financiera de TI](https://www.gartner.com/en/documents/3170717)