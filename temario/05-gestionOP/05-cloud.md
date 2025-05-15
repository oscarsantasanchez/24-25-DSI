# Computación en la nube

|Fundamentos|Infraestructura|Enfoques modernos|Gestión continua|
|-|-|-|-|
|[Gestión de Servicios de TI (ITSM)](01-itsm.md)|[Infraestructura tecnológica](03-infraestructura.md)|[DevOps y Site Reliability Engineering](06-devops-sre.md)|[Medición y mejora de servicios](07-medicion.md)|
|[Marcos de trabajo operativos: ITIL](02-itil.md)|[Servidores y su administración](04-servidores.md)|[Automatización operativa](09-automatizacion.md)|[Continuidad y recuperación](08-continuidad.md)|
||[**Computación en la nube**](05-cloud.md)|[Observabilidad y monitorización](10-observabilidad.md)|[Gobierno de servicios](11-gobierno.md)|

## ¿Por qué?

|Limitaciones de la infraestructura tradicional|Necesidad de agilidad y flexibilidad|Cambio en el modelo económico de TI|Globalización y movilidad|Innovación tecnológica acelerada|
|-|-|-|-|-|
|Las infraestructuras on-premise tradicionales presentan restricciones de escala, requieren grandes inversiones iniciales y tienen ciclos de renovación largos y costosos.|Las organizaciones necesitan adaptar rápidamente sus recursos tecnológicos a las cambiantes demandas del negocio y del mercado.|Evolución desde un modelo de inversión de capital (CapEx) hacia un modelo de gasto operativo (OpEx) más predecible y alineado con el uso real.|La expansión global de las organizaciones y la movilidad de los trabajadores exigen acceso a sistemas desde cualquier ubicación.|La velocidad de evolución tecnológica dificulta mantener infraestructuras propias actualizadas con las últimas capacidades disponibles.|

La computación en la nube surgió como respuesta a las crecientes limitaciones del modelo tradicional de TI. En un entorno empresarial caracterizado por la necesidad de mayor agilidad, escalabilidad y eficiencia económica, las restricciones inherentes a los centros de datos propios y la adquisición de hardware se volvieron obstáculos significativos. La nube representa una transformación fundamental en cómo se conciben, implementan y gestionan los recursos tecnológicos, pasando de activos físicos estáticos a servicios dinámicos consumidos según demanda.

## ¿Qué?

La computación en la nube es un modelo que permite el acceso bajo demanda a través de la red a un conjunto compartido de recursos informáticos configurables (redes, servidores, almacenamiento, aplicaciones y servicios) que pueden ser rápidamente aprovisionados y liberados con un mínimo esfuerzo de gestión o interacción del proveedor de servicios.

### Características esenciales

Según la definición del NIST (National Institute of Standards and Technology), la computación en la nube presenta cinco características fundamentales:

1. **Autoservicio bajo demanda**: Los usuarios pueden aprovisionar capacidades de computación según sus necesidades sin requerir interacción humana con el proveedor.

2. **Amplio acceso a la red**: Los servicios están disponibles a través de la red y son accesibles mediante mecanismos estándar que promueven el uso desde plataformas heterogéneas (móviles, tablets, portátiles, estaciones de trabajo).

3. **Agrupación de recursos**: Los recursos del proveedor se agrupan para servir a múltiples consumidores utilizando un modelo multi-inquilino, con diferentes recursos físicos y virtuales asignados dinámicamente según la demanda.

4. **Elasticidad rápida**: Las capacidades pueden aprovisionarse y liberarse de forma elástica, a veces incluso automáticamente, para escalar rápidamente en proporción a la demanda.

5. **Servicio medido**: Los sistemas en la nube controlan y optimizan automáticamente el uso de recursos mediante capacidades de medición a un nivel de abstracción apropiado para el tipo de servicio (almacenamiento, procesamiento, ancho de banda, usuarios activos).

### Modelos de servicio

<div align=center>

|Modelo|Descripción|Responsabilidad del cliente|Ejemplos|
|-|-|-|-|
|**SaaS (Software as a Service)**|Software completo accesible a través de la web, gestionado por el proveedor|Configuración de la aplicación y gestión de datos|Microsoft 365, Google Workspace, Salesforce, Workday|
|**PaaS (Platform as a Service)**|Plataforma para desarrollar, ejecutar y gestionar aplicaciones sin preocuparse por la infraestructura|Desarrollo y despliegue de aplicaciones|Azure App Service, Google App Engine, Heroku, AWS Elastic Beanstalk|
|**IaaS (Infrastructure as a Service)**|Recursos de infraestructura virtualizados bajo demanda|Gestión del SO y todo lo que se ejecuta sobre él|Amazon EC2, Azure Virtual Machines, Google Compute Engine|
|**CaaS (Container as a Service)**|Plataforma para gestionar y orquestar contenedores|Aplicaciones en contenedores y su configuración|Amazon ECS/EKS, Azure Container Instances, Google Kubernetes Engine|
|**FaaS (Function as a Service)**|Ejecución de funciones individuales en respuesta a eventos|Código de las funciones y su configuración|AWS Lambda, Azure Functions, Google Cloud Functions|

</div>

### Modelos de despliegue

<div align=center>

|Modelo|Características|Casos de uso típicos|
|-|-|-|
|**Nube pública**|• Propiedad de un proveedor externo<br>• Recursos compartidos entre múltiples clientes<br>• Accesible públicamente por Internet|Aplicaciones web públicas<br>Desarrollo y pruebas<br>Cargas de trabajo variables<br>Startups y experimentación|
|**Nube privada**|• Uso exclusivo de una organización<br>• Puede estar en instalaciones propias o del proveedor<br>• Mayor control y personalización|Datos sensibles o regulados<br>Aplicaciones críticas para el negocio<br>Organizaciones con altos requisitos de seguridad|
|**Nube híbrida**|• Combinación de nubes públicas y privadas<br>• Interconexión con posibilidad de portabilidad<br>• Balance entre control y flexibilidad|Extensión de capacidad (cloud bursting)<br>Separación de datos sensibles<br>Migración gradual a la nube|
|**Multi-nube**|• Uso de servicios de múltiples proveedores<br>• Sin necesidad de integración entre ellos<br>• Selección del mejor servicio de cada proveedor|Prevención de dependencia de proveedor<br>Requisitos específicos por servicio<br>Resiliencia mejorada|

</div>

### Principales proveedores de servicios en la nube

<div align=center>

|Proveedor|Servicios destacados|Diferenciadores|
|-|-|-|
|**Amazon Web Services (AWS)**|EC2, S3, Lambda, DynamoDB|Mayor catálogo de servicios<br>Presencia global extensa<br>Pionero en IaaS|
|**Microsoft Azure**|Virtual Machines, App Service, SQL Database|Integración con ecosistema Microsoft<br>Soluciones híbridas avanzadas<br>Enfoque empresarial|
|**Google Cloud Platform (GCP)**|Compute Engine, BigQuery, Kubernetes Engine|Fortaleza en análisis de datos y ML<br>Red global de alta velocidad<br>Innovación en contenedores|
|**IBM Cloud**|Watson, Cloudant, Cloud Foundry|Soluciones empresariales<br>IA y computación cuántica<br>Servicios de consultoría|

</div>

## ¿Para qué?

La adopción de la computación en la nube genera múltiples beneficios para las organizaciones:

### Beneficios económicos

- **Reducción de inversión inicial**: Eliminación o reducción significativa de gastos de capital (CapEx) en hardware y centros de datos.

- **Modelo basado en consumo**: Pago solo por los recursos utilizados, alineando costos con valor generado.

- **Predictibilidad financiera**: Mayor capacidad para presupuestar y gestionar gastos de TI.

- **Optimización de costos**: Herramientas y prácticas para identificar y eliminar gastos innecesarios.

- **Reducción del TCO**: Menor costo total de propiedad al eliminar gastos indirectos (espacio, refrigeración, electricidad).

### Beneficios operativos

- **Agilidad y velocidad**: Capacidad para aprovisionar recursos en minutos en lugar de semanas.

- **Escalabilidad elástica**: Adaptación automática a variaciones en la demanda, hacia arriba o hacia abajo.

- **Disponibilidad mejorada**: Arquitecturas diseñadas para alta disponibilidad con SLAs garantizados.

- **Alcance global**: Despliegue de servicios en múltiples regiones geográficas sin infraestructura propia.

- **Recuperación ante desastres**: Capacidades mejoradas para continuidad del negocio y recuperación.

- **Actualizaciones automáticas**: Mantenimiento continuo realizado por el proveedor sin interrupciones significativas.

### Beneficios estratégicos

- **Enfoque en diferenciación**: Liberación de recursos para concentrarse en actividades de valor agregado.

- **Innovación acelerada**: Acceso inmediato a tecnologías emergentes sin inversiones adicionales.

- **Experimentación con bajo riesgo**: Capacidad para probar nuevas ideas con inversión mínima.

- **Transformación digital**: Facilitación de nuevos modelos de negocio digitales.

- **Ventaja competitiva**: Mayor capacidad de respuesta a cambios del mercado.

## ¿Cómo?

### Estrategias de adopción de la nube

<div align=center>

|Estrategia|Descripción|Cuándo es apropiada|
|-|-|-|
|**Lift & Shift (Rehosting)**|Migración directa de aplicaciones a la nube sin cambios significativos|• Necesidad de salir rápidamente de un centro de datos<br>• Aplicaciones con poca necesidad de optimización<br>• Primer paso en una estrategia por fases|
|**Refactorización (Replatforming)**|Modificaciones moderadas para aprovechar algunas ventajas de la nube|• Balance entre velocidad y optimización<br>• Aplicaciones con componentes fácilmente adaptables<br>• Camino intermedio en la transformación|
|**Rediseño (Rearchitecting)**|Rediseño significativo para explotar plenamente características nativas de la nube|• Aplicaciones estratégicas a largo plazo<br>• Necesidades claras de escalabilidad o rendimiento<br>• Competencia en mercados digitales|
|**Reconstrucción (Rebuilding)**|Desarrollo completamente nuevo utilizando servicios nativos de la nube|• Aplicaciones obsoletas técnicamente<br>• Cambios fundamentales en requisitos<br>• Oportunidades para innovación disruptiva|
|**Reemplazo (Replacing)**|Abandono de aplicaciones propias por soluciones SaaS|• Funcionalidades no diferenciadoras<br>• Disponibilidad de soluciones maduras en el mercado<br>• Reducción de costos de desarrollo y mantenimiento|

</div>

### El recorrido hacia la nube

La adopción de la nube generalmente sigue un proceso evolutivo con varias etapas:

1. **Evaluación y planificación**:
   - Análisis del portafolio de aplicaciones
   - Establecimiento de caso de negocio
   - Definición de hoja de ruta
   - Selección de proveedores y servicios

2. **Fundamentos y gobernanza**:
   - Establecimiento de estructura organizativa
   - Definición de políticas y controles
   - Configuración de redes y conectividad
   - Implementación de seguridad básica

3. **Migración inicial**:
   - Priorización de cargas de trabajo
   - Pruebas de concepto
   - Implementación de estrategias de migración
   - Validación y optimización inicial

4. **Escalado y optimización**:
   - Expansión a más aplicaciones
   - Adopción de más servicios nativos
   - Automatización de operaciones
   - Optimización de costos y rendimiento

5. **Transformación e innovación**:
   - Rediseño para arquitecturas nativas de nube
   - Desarrollo de nuevos modelos de negocio
   - Implementación de analítica avanzada e IA
   - Optimización continua

### Arquitecturas para la nube

Las arquitecturas en la nube difieren significativamente de las tradicionales, adoptando principios específicos:

1. **Diseño para fallos**: Asumir que los componentes fallarán y diseñar sistemas resilientes.

2. **Acoplamiento débil**: Componentes autónomos que se comunican a través de interfaces bien definidas.

3. **Diseño para elasticidad**: Capacidad de escalar horizontal y verticalmente según demanda.

4. **Inmutabilidad**: En lugar de actualizar componentes existentes, reemplazarlos por nuevos.

5. **Infraestructura como código**: Definir toda la infraestructura mediante código versionable.

6. **Automatización completa**: Despliegue, escalado, recuperación y pruebas automatizadas.

7. **Stateless cuando sea posible**: Minimizar el estado mantenido en servidores de aplicación.

8. **Seguridad en cada capa**: Implementar defensas a nivel de red, aplicación y datos.

### Gestión de costos en la nube

El modelo financiero de la nube requiere nuevos enfoques para gestionar y optimizar costos:

<div align=center>

|Estrategia|Descripción|Prácticas recomendadas|
|-|-|-|
|**Visibilidad y asignación**|Comprender y atribuir costos a unidades organizativas|• Etiquetado consistente<br>• Presupuestos por unidad<br>• Dashboards de costos<br>• Reportes regulares|
|**Dimensionamiento adecuado**|Ajustar recursos al nivel realmente necesario|• Análisis de utilización<br>• Recomendaciones de tamaño<br>• Familia de instancias adecuada<br>• Ajuste de bases de datos|
|**Elasticidad**|Escalar recursos según demanda actual|• Auto-scaling<br>• Apagado automático<br>• Programación por horarios<br>• Instancias efímeras|
|**Selección de servicios**|Elegir los servicios más costo-efectivos|• Compromiso vs bajo demanda<br>• Servicios gestionados<br>• Tecnologías sin servidor<br>• Análisis de alternativas|

</div>

### Seguridad en la nube

La seguridad en entornos cloud requiere un enfoque compartido entre proveedor y cliente:

<div align=center>

|Modelo de servicio|Responsabilidad del proveedor|Responsabilidad del cliente|
|-|-|-|
|**SaaS**|• Toda la infraestructura<br>• Aplicación y su seguridad<br>• Parches y actualizaciones|• Gestión de usuarios y accesos<br>• Seguridad de datos<br>• Configuración de controles|
|**PaaS**|• Infraestructura física<br>• Sistemas operativos<br>• Componentes de plataforma|• Aplicaciones desplegadas<br>• Integración<br>• Gestión de identidades|
|**IaaS**|• Hardware físico<br>• Virtualización<br>• Seguridad perimetral<br>• Red troncal|• Sistemas operativos<br>• Configuración de red<br>• Datos y aplicaciones<br>• Gestión de parches|

</div>

Las principales áreas de enfoque para la seguridad en la nube incluyen:

1. **Gestión de identidades y accesos**: Implementación de principio de mínimo privilegio, autenticación multifactor, gestión de identidades privilegiadas.

2. **Seguridad de datos**: Clasificación, cifrado, tokenización, gestión de claves, prevención de pérdida de datos.

3. **Seguridad de red**: Segmentación, firewalls, grupos de seguridad, inspección de tráfico, VPN, detección de intrusiones.

4. **Seguridad de aplicaciones**: Desarrollo seguro, análisis de vulnerabilidades, WAF, gestión de dependencias.

5. **Monitorización y detección**: Logs centralizados, análisis de comportamiento, alertas, respuesta a incidentes.

6. **Cumplimiento y gobernanza**: Políticas, controles, auditorías, alineación con marcos regulatorios.

### Operaciones en la nube

La gestión de entornos cloud requiere nuevos enfoques operativos:

1. **Cloud Operations (CloudOps)**: Procesos y herramientas específicos para entornos cloud, con énfasis en automatización, observabilidad y gestión de recursos dinámicos.

2. **Financial Operations (FinOps)**: Disciplina que combina finanzas, operaciones y tecnología para gestionar y optimizar el gasto en la nube.

3. **DevSecOps en la nube**: Integración de seguridad en ciclos de desarrollo y operaciones, con herramientas nativas de los proveedores.

4. **Site Reliability Engineering (SRE)**: Aplicación de principios de ingeniería de software a operaciones de infraestructura.

## Tendencias y evolución

La computación en la nube continúa evolucionando rápidamente en varias direcciones:

### Tendencias emergentes

1. **Edge Computing**: Extensión de la nube hacia el borde de la red, más cerca de donde se generan y consumen los datos.

2. **Serverless y Event-Driven**: Abstracción completa de la infraestructura, con ejecución basada en eventos y pago por uso real.

3. **IA y ML como servicio**: Democratización de capacidades avanzadas de inteligencia artificial sin necesidad de experiencia profunda.

4. **Plataformas de bajo código/sin código**: Capacidades para desarrollar soluciones sin programación tradicional.

5. **Multicloud avanzado**: Servicios y plataformas que facilitan la gestión coherente entre múltiples proveedores.

### Desafíos persistentes

A pesar de su madurez, la nube sigue presentando desafíos significativos:

1. **Dependencia de proveedor (vendor lock-in)**: Dificultad para migrar entre proveedores una vez adoptados servicios nativos.

2. **Complejidad de gestión**: Entornos multi-nube y redes globales con numerosos servicios y configuraciones.

3. **Cumplimiento normativo**: Reglas cambiantes sobre soberanía de datos, privacidad y responsabilidad.

4. **Brechas de habilidades**: Escasez de profesionales con experiencia en tecnologías cloud avanzadas.

5. **Costos imprevistos**: Gastos no planificados debido a consumo no controlado o mal entendido.

## Enlaces y referencias

- [NIST Cloud Computing Program](https://www.nist.gov/programs-projects/nist-cloud-computing-program-nccp)
- [Cloud Security Alliance](https://cloudsecurityalliance.org/)
- [AWS Architecture Center](https://aws.amazon.com/architecture/)
- [Microsoft Azure Architecture Center](https://docs.microsoft.com/en-us/azure/architecture/)
- [Google Cloud Architecture Framework](https://cloud.google.com/architecture/framework)
- [FinOps Foundation](https://www.finops.org/)