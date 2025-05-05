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
</style>

# Operaciones y Servicios<br>de Sistemas de Información

### Gestión y mantenimiento de servicios de TI

---

## Agenda

1. **Introducción**: ¿Por qué son importantes las operaciones?
2. **Fundamentos de la gestión de servicios**
   - Gestión de Servicios de TI (ITSM)
   - Marco ITIL
3. **Infraestructura tecnológica**
   - Servidores y administración
   - Computación en la nube
4. **Casos prácticos y discusión**

---

## ¿Por qué operaciones?

![bg right:35% 80%](https://images.unsplash.com/photo-1550751827-4bd374c3f58b?w=800)

La mejor estrategia y el proyecto mejor ejecutado **fracasan** sin una operación adecuada que mantenga los sistemas funcionando correctamente día a día.

---

## El desafío operativo

<div class="columns">
<div>

### Complejidad creciente

- Entornos locales
- Servicios cloud
- Aplicaciones de terceros  
- Desarrollos propios

</div>
<div>

### Impacto del downtime

- Detención de actividad
- Multiplica costos por minuto
- Daño de reputación
- Pérdida de oportunidades

</div>
</div>

---

## ¿Qué son las operaciones de TI?

> Prácticas, procesos y actividades necesarias para **entregar, mantener y optimizar** de manera continua los servicios tecnológicos.

<div class="columns-3">
<div>

### Gestión de servicios
- ITIL, COBIT
- SLAs
- Incidentes

</div>
<div>

### Infraestructura  
- Servidores
- Redes
- Cloud

</div>
<div>

### Entrega continua
- Monitorización
- Automatización
- Disponibilidad

</div>
</div>

---


## El ciclo PODC en operaciones

|Fase|Actividades|Conexión|
|-|-|-|
|**Planificar**|Diseño de servicios, Capacidad|→ Estrategia|
|**Organizar**|Implementación, Configuración|→ Equipos|
|**Dirigir**|Operación diaria, Incidentes|→ Liderazgo|
|**Controlar**|Monitorización, Mejora|→ Métricas|

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
- Imposible operar sin ella

</div>
<div>

### Complejidad organizacional
- Sistemas heredados
- Soluciones actuales  
- Tecnologías emergentes

</div>
</div>

---

## Elementos fundamentales ITSM

|Elemento|Descripción|
|-|-|
|**Servicios**|Entregar valor sin que los usuarios asuman costos/riesgos|
|**Procesos**|Actividades estructuradas con entradas/salidas definidas|
|**Roles**|Definición clara de responsabilidades|
|**SLAs**|Compromisos de calidad y disponibilidad|
|**Catálogo**|Inventario centralizado de servicios|

---

## SLA

![bg center:30% 50%](https://www.servicetonic.com/wp-content/uploads/2016/12/ejemplo-de-un-buen-SLA.png)

---

## Áreas clave de ITSM

<div class="columns">
<div>

### Reactivas
- Gestión de incidentes
- Resolución de problemas  
- Restauración de servicios

</div>
<div>

### Proactivas  
- Gestión de cambios
- Gestión de la capacidad
- Gestión de la disponibilidad

</div>
</div>

---

# Marco ITIL

## Information Technology Infrastructure Library

![bg right:35% 80%](https://cdn.ttgtmedia.com/rms/onlineImages/enterprise_wms-19-itil-dimensions-f_mobile.png)

---

## Evolución de ITIL

|Versión|Año|Enfoque|
|-|-|-|
|**ITIL v1**|1989-1995|Operaciones de TI|
|**ITIL v2**|2000-2006|Procesos de servicio|
|**ITIL v3**|2007-2011|Ciclo de vida del servicio|
|**ITIL 4**|2019-presente|Valor y transformación digital|

---

## ITIL 4: Sistema de Valor

<div class="columns">
<div>

### Principios guía
1. Enfocarse en el valor
2. Comenzar donde estás
3. Progresar iterativamente
4. Colaborar y promover visibilidad
5. Pensar holísticamente

</div>
<div>

### Cadena de valor
- Planificar
- Mejorar
- Asegurar
- Entregar
- Obtener/construir

</div>
</div>

---

## Prácticas de ITIL 4

<div class="columns-3">
<div>

### Gestión general
- Estrategia
- Seguridad
- Finanzas
- Conocimiento

</div>
<div>

### Gestión de servicios
- Mesa de servicio
- Incidentes
- Problemas
- Cambios
- SLAs

</div>
<div>

### Gestión técnica  
- Despliegues
- Infraestructura
- Desarrollo
- Arquitectura

</div>
</div>

---

## Certificaciones ITIL

|Nivel|Enfoque|Dirigido a|
|-|-|-|
|**Foundation**|Conceptos básicos|Todos los profesionales|
|**Managing Professional**|Habilidades prácticas|Gestores de servicios|
|**Strategic Leader**|Liderazgo estratégico|Directivos|
|**Master**|Dominio avanzado|Expertos|

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
- Crecimiento demanda
- Optimización costos
- Seguridad y control

</div>
</div>

---

## Componentes de infraestructura

|Componente|Descripción|Ejemplos|
|-|-|-|
|**Hardware**|Equipos físicos|Servidores, switches, storage|
|**Software base**|Control de recursos|SO, middleware, DBMS|
|**Redes**|Comunicación de datos|LAN/WAN, VPN, firewalls|
|**Instalaciones**|Espacios físicos|Centros de datos, UPS|

---

## Modelos de infraestructura

<div class="columns">
<div>

### Tradicional
- On-premise
- Control total
- Ciclos largos

</div>
<div>

### Cloud
- Recursos a demanda
- Escalabilidad
- Pago por uso

</div>
</div>

---

## Tendencias en infraestructura

1. **Virtualización** → Contenedores
2. **Automación** → IAC (Infrastructure as Code)
3. **Edge Computing** → Procesamiento local
4. **Sostenibilidad** → Green IT
5. **IA/ML** → Gestión inteligente

---

# Servidores

## El corazón de la infraestructura

![bg right:40% 90%](https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=800)

---

## Tipos de servidores

<div class="columns">
<div>

### Por implementación
- Físicos dedicados
- Virtualizados
- En la nube
- Contenedores
- Serverless

</div>
<div>

### Por función
- Web servers
- Database servers
- Application servers
- File servers
- DNS servers

</div>
</div>

---

## Ciclo de administración

|Fase|Actividades|
|-|-|
|**Planificación**|Requisitos, diseño, dimensionamiento|
|**Implementación**|Instalación, configuración, testing|
|**Operación**|Monitorización, mantenimiento, parches|
|**Optimización**|Rendimiento, capacidad, actualizaciones|
|**Retirada**|Migración, backup, desmantelamiento|

---

## Gestión de servidores: Desafíos

<div class="columns">
<div>

### Proliferación
- Crecimiento descontrolado
- Gestión manual insostenible

</div>
<div>

### Parches
- Actualizaciones críticas
- Ventanas de mantenimiento

</div>
</div>

<div class="columns">
<div>

### Monitorización
- Balance de alertas
- Datos relevantes

</div>
<div>

### Seguridad
- Hardening
- Control de accesos

</div>
</div>

---

# Computación en la Nube

## La infraestructura del futuro

![bg right:35% 90%](https://cdn-icons-png.flaticon.com/512/4215/4215831.png)

---

## ¿Por qué cloud?

<div class="columns">
<div>

### Limitaciones tradicionales
- Inversiones altas
- Ciclos largos
- Poca flexibilidad

</div>
<div>

### Ventajas cloud
- Agilidad
- Escalabilidad
- CapEx → OpEx

</div>
</div>

---

## Características esenciales

1. **Autoservicio bajo demanda**
2. **Amplio acceso a red**  
3. **Recursos compartidos**
4. **Elasticidad rápida**
5. **Servicio medido**

---

## Modelos de servicio

|Modelo|Concepto|Cliente responsable de|Ejemplos|
|-|-|-|-|
|**SaaS**|Software como servicio|Datos y configuración|Office 365, Salesforce|
|**PaaS**|Plataforma como servicio|Aplicaciones|Azure App Service|
|**IaaS**|Infraestructura como servicio|SO y arriba|AWS EC2, Azure VMs|

---

## Cloud: Beneficios económicos

<div class="columns">
<div>

### Financieros
- Sin inversión inicial
- Pago por uso
- TCO reducido
- Costos predictivos

</div>
<div>

### Operativos  
- Aprovisionamiento rápido
- Auto-scaling
- Global reach
- 24/7 availability

</div>
</div>

---

## Cloud: Adopción exitosa

### Estrategias
1. **Lift & Shift** → Migración directa
2. **Replatform** → Modificación moderada  
3. **Refactor** → Rediseño nativo cloud
4. **Replace** → Soluciones SaaS

---

# Casos de estudio

## Operaciones en acción

---

## Caso 1: Incidente crítico

**Situación**: Caída del servidor de base de datos principal

**Elementos ITSM implicados**:
- Gestión de incidentes
- Gestión de la disponibilidad
- Gestión de la configuración

**Infraestructura involucrada**:
- Servidores database
- Sistemas de backup
- Failover systems

---

## Caso 2: Migración a cloud

**Escenario**: Empresa retail migra 200 servidores a AWS

**Marcos aplicados**:
- ITIL para gestión de cambios
- IaC para configuración

**Resultados**:
- 60% reducción costos
- Disponibilidad de 99.9%
- Tiempo de despliegue -80%

---

# Integración de conceptos

## Conectando los puntos

---

## ITSM + Infraestructura

<div class="columns">
<div>

### Antes
- Gestión reactiva
- Procesos manuales
- Infraestructura estática

</div>
<div>

### Ahora
- ITSM + cloud-native
- Automatización
- Infraestructura dinámica

</div>
</div>

---

## Cloud-native operations

```
ITSM tradicional + Cloud = Nueva generación operativa

• DevOps integrado con ITIL
• IaC para gestión de configuración
• Observabilidad for incident management
• Auto-scaling for capacity management
```

---

# Conclusiones

## Puntos clave

---

## 1. Evolución operativa

**De**: Gestión reactiva y manual  
**A**: Proactivo, automatizado, cloud-native

**Clave**: Adoptar marcos como ITIL mientras se evoluciona

---

## 2. Infraestructura moderna

**Combinación ganadora**:
- Bases ITSM sólidas
- Infraestructura flexible  
- Automatización inteligente

---

## 3. El futuro es híbrido

<div class="columns">
<div>

### Mix perfecto
- On-premise crítico
- Cloud para escalabilidad  
- Edge para latencia
- Multi-cloud para resiliencia

</div>
<div>

### Skills necesarias
- ITIL/DevOps
- Cloud arquitectura
- Automatización
- Seguridad operativa

</div>
</div>

---

# Recursos adicionales

- [ITIL 4 Foundation](https://www.axelos.com/certifications/itil-certifications/itil-foundation)
- [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected/)
- [Google SRE Book](https://sre.google/sre-book/table-of-contents/)
- [Kubernetes Documentation](https://kubernetes.io/docs/home/)