# Servidores y su administración

|Fundamentos|Infraestructura|Enfoques modernos|Gestión continua|
|-|-|-|-|
|[Gestión de Servicios de TI (ITSM)](01-itsm.md)|[Infraestructura tecnológica](03-infraestructura.md)|[DevOps y Site Reliability Engineering](06-devops-sre.md)|[Medición y mejora de servicios](07-medicion.md)|
|[Marcos de trabajo operativos: ITIL](02-itil.md)|[**Servidores y su administración**](04-servidores.md)|[Automatización operativa](09-automatizacion.md)|[Continuidad y recuperación](08-continuidad.md)|
||[Computación en la nube](05-cloud.md)|[Observabilidad y monitorización](10-observabilidad.md)|[Gobierno de servicios](11-gobierno.md)|

## ¿Por qué?

|Centralización de recursos|Procesamiento de cargas críticas|Especialización de funciones|Eficiencia y escalabilidad|Seguridad y control|
|-|-|-|-|-|
|La necesidad de centralizar recursos informáticos para optimizar su utilización y facilitar su gestión.|El requerimiento de sistemas dedicados capaces de procesar cargas de trabajo específicas con alto rendimiento y disponibilidad.|La diversificación de servicios digitales exige sistemas especializados para cada función (bases de datos, aplicaciones, webs).|El crecimiento de usuarios y volumen de datos demanda sistemas diseñados para escalar y operar eficientemente.|La necesidad de establecer entornos controlados y seguros para información sensible y procesos críticos.|

Los servidores constituyen la columna vertebral de los entornos informáticos empresariales, evolucionando desde las primeras máquinas centralizadas hasta las complejas arquitecturas distribuidas actuales. La tendencia hacia la digitalización ha multiplicado tanto la cantidad como la variedad de servicios que las organizaciones necesitan proporcionar, haciendo que la correcta selección, configuración y administración de servidores sea un factor determinante para la eficiencia operativa, la continuidad del negocio y la capacidad de innovación.

## ¿Qué?

Un servidor es un sistema informático físico o virtual diseñado para proporcionar servicios, recursos o funcionalidades a otros sistemas, aplicaciones o usuarios (denominados "clientes") a través de una red. Los servidores están optimizados para ejecutar cargas de trabajo específicas de manera eficiente, confiable y segura.

### Tipos de servidores según implementación física

<div align=center>

|Tipo|Descripción|Características|
|-|-|-|
|**Servidores físicos dedicados**|Hardware físico específicamente diseñado para función de servidor|Hardware especializado y robusto<br>Completo aislamiento de recursos<br>Control total sobre el entorno|
|**Servidores virtualizados**|Múltiples servidores virtuales funcionando sobre hardware físico compartido|Mejor aprovechamiento de recursos<br>Aislamiento lógico entre instancias<br>Mayor flexibilidad y portabilidad|
|**Servidores en la nube**|Instancias de servidor proporcionadas como servicio por proveedores cloud|Escalabilidad dinámica<br>Modelo de pago por uso<br>Reducción de gestión de infraestructura|
|**Servidores en contenedores**|Aplicaciones y dependencias empaquetadas en contenedores ligeros|Despliegue ultrarrápido<br>Alta densidad de aplicaciones<br>Portabilidad entre entornos|
|**Servidores sin servidor (serverless)**|Funciones que se ejecutan en respuesta a eventos sin gestionar infraestructura|Escalado automático<br>Cobro por ejecución real<br>Sin administración de servidores|

</div>

### Tipos de servidores según función

<div align=center>

|Tipo|Función principal|Ejemplos|
|-|-|-|
|**Servidores web**|Entregar contenido web a navegadores y aplicaciones|Apache, Nginx, IIS, Tomcat|
|**Servidores de aplicaciones**|Ejecutar lógica de negocio para aplicaciones|WebSphere, WebLogic, JBoss, .NET|
|**Servidores de bases de datos**|Almacenar, recuperar y gestionar datos estructurados|SQL Server, Oracle, MySQL, PostgreSQL|
|**Servidores de archivos**|Almacenar y compartir archivos en la red|Windows File Server, NAS, Samba|
|**Servidores de correo**|Gestionar envío, recepción y almacenamiento de correos|Exchange, Postfix, Sendmail, Zimbra|
|**Servidores de autenticación**|Validar identidades y gestionar accesos|Active Directory, LDAP, Kerberos|
|**Servidores de DNS**|Resolver nombres de dominio a direcciones IP|BIND, Windows DNS, dnsmasq|
|**Servidores de virtualización**|Gestionar múltiples máquinas virtuales|VMware ESXi, Hyper-V, KVM|
|**Servidores de backup**|Gestionar copias de seguridad y recuperación|Veeam, Commvault, Backup Exec|
|**Servidores de monitorización**|Supervisar el estado y rendimiento de sistemas|Nagios, Zabbix, PRTG, Prometheus|

</div>

### Componentes de un servidor

<div align=center>

|Componente|Función|Consideraciones de rendimiento|
|-|-|-|
|**CPU (Procesador)**|Ejecutar instrucciones y procesar datos|Número de núcleos/hilos<br>Velocidad de reloj<br>Caché<br>Arquitectura (x86, ARM, etc.)|
|**Memoria RAM**|Almacenamiento temporal para datos en uso|Capacidad total<br>Velocidad<br>Tipo (DDR4, DDR5)<br>ECC para protección de errores|
|**Almacenamiento**|Guardar datos y programas persistentemente|Tipo (HDD, SSD, NVMe)<br>Capacidad<br>RAID para redundancia<br>Velocidad de acceso|
|**Tarjetas de red**|Comunicación con otros sistemas|Ancho de banda (1G, 10G, etc.)<br>Redundancia<br>Características especiales (TOE, RDMA)|
|**Sistema operativo**|Software que controla el hardware y proporciona servicios|Windows Server<br>Linux (varias distribuciones)<br>FreeBSD<br>VMware ESXi|
|**Fuentes de alimentación**|Suministrar energía al sistema|Potencia adecuada<br>Redundancia<br>Eficiencia energética|
|**Sistemas de refrigeración**|Mantener temperaturas operativas adecuadas|Ventiladores<br>Refrigeración líquida<br>Diseño térmico|

</div>

## ¿Para qué?

Los servidores cumplen funciones críticas en las organizaciones modernas:

### Centralización y optimización

- **Consolidación de recursos**: Concentración de capacidad de cómputo para mejor aprovechamiento.
- **Estandarización**: Plataformas comunes que facilitan la gestión y el soporte.
- **Economías de escala**: Reducción de costos mediante uso eficiente de recursos compartidos.
- **Gestión centralizada**: Administración unificada que mejora control y visibilidad.

### Habilitación de servicios críticos

- **Aplicaciones corporativas**: Plataformas para ERP, CRM, colaboración, etc.
- **Servicios de infraestructura**: DNS, DHCP, directorio activo, etc.
- **Plataformas web y e-commerce**: Sitios web, tiendas online, portales.
- **Análisis de datos**: Procesamiento de grandes volúmenes de información.
- **Servicios de comunicación**: Correo electrónico, mensajería, videoconferencia.

### Protección y continuidad

- **Seguridad de datos**: Entornos controlados con medidas de protección rigurosas.
- **Copias de seguridad**: Mecanismos para preservar y recuperar información.
- **Recuperación ante desastres**: Capacidades para restaurar operaciones tras incidentes.
- **Alta disponibilidad**: Configuraciones que minimizan tiempos de inactividad.

### Evolución y crecimiento

- **Escalabilidad**: Capacidad para crecer según demanda del negocio.
- **Plataforma para innovación**: Base para desarrollo y prueba de nuevas iniciativas.
- **Adaptación tecnológica**: Integración de nuevas tecnologías y enfoques.

## ¿Cómo?

La administración efectiva de servidores abarca múltiples dimensiones:

### Ciclo de vida de la administración de servidores

<div align=center>

|Fase|Actividades principales|
|-|-|
|**Planificación**|Análisis de requisitos<br>Selección de plataformas<br>Diseño de arquitectura<br>Dimensionamiento|
|**Implementación**|Instalación física/virtual<br>Configuración básica<br>Instalación de sistema operativo<br>Hardening de seguridad|
|**Configuración**|Instalación de software y servicios<br>Configuración de red<br>Integración con sistemas existentes<br>Pruebas de funcionamiento|
|**Operación**|Monitorización proactiva<br>Gestión de rendimiento<br>Aplicación de parches<br>Resolución de incidentes|
|**Optimización**|Análisis de capacidad<br>Ajuste de rendimiento<br>Actualización de componentes<br>Consolidación cuando sea apropiado|
|**Retirada**|Planificación de migración<br>Copia de seguridad de datos<br>Desmantelamiento seguro<br>Eliminación segura de información|

</div>

### Administración de servidores físicos

La gestión de servidores físicos requiere atención a aspectos específicos del hardware:

1. **Gestión del hardware**:
   - Monitorización de componentes (temperaturas, ventiladores, fuentes de alimentación)
   - Diagnóstico y resolución de problemas físicos
   - Actualización de firmware y controladores
   - Gestión de garantías y contratos de soporte

2. **Consideraciones de instalaciones**:
   - Refrigeración adecuada
   - Suministro eléctrico estable (incluye UPS, generadores)
   - Seguridad física
   - Cableado estructurado

3. **Sistemas de gestión remota**:
   - Tecnologías como IPMI, iDRAC, iLO
   - Consolas KVM sobre IP
   - Acceso de emergencia fuera de banda

### Administración de servidores virtuales

La virtualización ha transformado la administración de servidores:

1. **Gestión de hipervisores**:
   - Configuración de hosts
   - Gestión de recursos compartidos
   - Optimización de rendimiento
   - Actualizaciones y parches

2. **Gestión de máquinas virtuales**:
   - Aprovisionamiento y despliegue
   - Clonación y plantillas
   - Snapshots y copias de seguridad
   - Migración entre hosts

3. **Optimización de entornos virtuales**:
   - Balanceo de carga entre hosts
   - Deduplicación y thin provisioning
   - Gestión de sobresuscripción
   - Monitorización específica de virtualización

### Administración de sistemas operativos de servidor

Independientemente del tipo de implementación, la gestión del sistema operativo es fundamental:

<div align=center>

|Aspecto|Actividades principales|
|-|-|
|**Gestión de usuarios y permisos**|Creación y mantenimiento de cuentas<br>Asignación de permisos<br>Implementación de políticas de contraseñas<br>Auditoría de accesos|
|**Gestión de actualizaciones**|Evaluación de parches y actualizaciones<br>Pruebas en entornos no productivos<br>Planificación de ventanas de mantenimiento<br>Implementación controlada|
|**Configuración de red**|Direccionamiento IP<br>Configuración de firewalls<br>Routing y switching<br>Monitorización de tráfico|
|**Gestión de almacenamiento**|Particionamiento y formateo<br>Configuración de RAID<br>Monitorización de espacio<br>Optimización de rendimiento|
|**Monitorización y logs**|Configuración de herramientas de monitorización<br>Recolección centralizada de logs<br>Alertas y notificaciones<br>Análisis de tendencias|
|**Copias de seguridad**|Configuración de políticas de respaldo<br>Verificación de backups<br>Pruebas de restauración<br>Retención de datos|

</div>

### Automatización y gestión a escala

En entornos con múltiples servidores, la automatización se vuelve esencial:

1. **Herramientas de gestión de configuración**:
   - Ansible, Puppet, Chef, SaltStack
   - Definición declarativa de estados deseados
   - Control de versiones de configuraciones
   - Despliegue consistente a múltiples servidores

2. **Infraestructura como código (IaC)**:
   - Terraform, CloudFormation, ARM Templates
   - Definición programática de infraestructura
   - Reproducibilidad y consistencia
   - Integración con control de versiones

3. **Orquestación de contenedores**:
   - Kubernetes, Docker Swarm, OpenShift
   - Despliegue automatizado
   - Escalado dinámico
   - Auto-reparación

### Seguridad de servidores

La protección de servidores es un aspecto crítico de su administración:

<div align=center>

|Área|Prácticas recomendadas|
|-|-|
|**Hardening**|Eliminar servicios innecesarios<br>Aplicar configuraciones seguras<br>Implementar principio de mínimo privilegio<br>Deshabilitar cuentas predeterminadas|
|**Parcheado**|Mantener actualizaciones de seguridad<br>Proceso formal de gestión de parches<br>Verificación de aplicación correcta<br>Ventanas de mantenimiento programadas|
|**Control de acceso**|Autenticación multifactor<br>Gestión centralizada de identidades<br>Rotación de credenciales<br>Registros de auditoría|
|**Protección de red**|Segmentación y microsegmentación<br>Firewalls y sistemas de detección de intrusiones<br>Cifrado de comunicaciones<br>Monitorización de tráfico anómalo|
|**Protección de datos**|Cifrado de datos sensibles<br>Gestión segura de claves<br>Controles de acceso a datos<br>Prevención de fuga de información|
|**Monitorización de seguridad**|Recolección centralizada de logs<br>Análisis de eventos de seguridad<br>Detección de comportamientos anómalos<br>Correlación de eventos|
|**Gestión de vulnerabilidades**|Escaneos regulares<br>Evaluación de riesgos<br>Remediación priorizada<br>Pruebas de penetración|

</div>

### Tendencias actuales en administración de servidores

La forma de administrar servidores está evolucionando rápidamente:

1. **Servidores inmutables**: En lugar de actualizar servidores existentes, se reemplazan completamente por nuevas instancias con la configuración actualizada.

2. **Administración basada en API**: Gestión de todos los aspectos del servidor a través de APIs programáticas en lugar de interfaces gráficas.

3. **Gestión como código**: Definición declarativa de la configuración deseada versionada en repositorios de código.

4. **Observabilidad avanzada**: Más allá de la monitorización tradicional, capturando métricas, logs y trazas para entender completamente el comportamiento.

5. **Automatización inteligente**: Uso de IA para predecir problemas, optimizar rendimiento y automatizar tareas rutinarias.

## Desafíos y mejores prácticas

### Desafíos comunes

<div align=center>

|Desafío|Descripción|Mejores prácticas|
|-|-|-|
|**Proliferación de servidores**|Crecimiento descontrolado de servidores que dificulta gestión|Inventario centralizado<br>Políticas de aprovisionamiento<br>Consolidación y racionalización|
|**Inconsistencia de configuraciones**|Variaciones no controladas entre servidores similares|Automatización de configuración<br>Plantillas de referencia<br>Auditorías regulares|
|**Gestión de parches**|Dificultad para mantener sistemas actualizados y seguros|Proceso formal de parcheado<br>Entornos de prueba<br>Automatización de despliegue|
|**Monitorización efectiva**|Balance entre exceso y falta de datos de monitorización|Definición clara de métricas clave<br>Alertas significativas<br>Eliminación de ruido|
|**Escalabilidad**|Crecimiento que supera capacidad de gestión manual|Automatización<br>Estandarización<br>Arquitecturas elásticas|
|**Respaldo y recuperación**|Asegurar protección de datos en servidores críticos|Estrategia 3-2-1 de backups<br>Pruebas regulares<br>Automatización de respaldos|

</div>

### Mejores prácticas generales

1. **Documentación**: Mantener documentación actualizada de configuraciones, procedimientos y topología.

2. **Estandarización**: Establecer configuraciones estándar y minimizar variaciones innecesarias.

3. **Automatización**: Automatizar tareas repetitivas para reducir errores y mejorar eficiencia.

4. **Testing**: Probar cambios en entornos no productivos antes de aplicarlos en producción.

5. **Monitorización proactiva**: Implementar alertas que permitan prevenir problemas, no solo detectarlos.

6. **Gestión de capacidad**: Planificar proactivamente para evitar problemas de rendimiento.

7. **Seguridad por capas**: Implementar defensas múltiples y redundantes.

8. **Gestión del conocimiento**: Promover transferencia de conocimiento para evitar dependencia de individuos.

## Enlaces y referencias

- [Microsoft Windows Server Documentation](https://docs.microsoft.com/en-us/windows-server/)
- [Red Hat Enterprise Linux Documentation](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/)
- [VMware vSphere Documentation](https://docs.vmware.com/en/VMware-vSphere/)
- [The Debian Administrator's Handbook](https://debian-handbook.info/)
- [Center for Internet Security (CIS) Benchmarks](https://www.cisecurity.org/cis-benchmarks/)
- [NIST Special Publication 800-123: Guide to General Server Security](https://csrc.nist.gov/publications/detail/sp/800-123/final)
- [Kubernetes Documentation](https://kubernetes.io/docs/home/)