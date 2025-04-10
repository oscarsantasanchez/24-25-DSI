# GdPyIS > Arquitecturas de integración de sistemas

|Herramientas|Diseño|Implantación|Valoración|
|-|-|-|-|
|[Lenguajes de programación](lenguajesProgramacion.md)|[Evaluación de requisitos y selección de sistemas](requisitos.md)|[Gestión del cambio y adopción del usuario](gestionDelCambio.md)|[Indicadores](indicadores.md)|
|[NoCode](noCode.md)|[**Arquitectura de integración de sistemas**](arquitectura.md)|[Gestión de la seguridad e integridad de datos](gestionSeguridad.md)|[Gestión de riesgos](riesgos.md)|
|[Metodologías de desarrollo](metodologiasDesarrollo.md)
|[Tipología de aplicaciones](tipologia.md)
|[Sistemas ERP (Enterprise Resource Planning)](erp.md)

## ¿Por qué?

La arquitectura de integración de sistemas es fundamental para asegurar un flujo de información coherente entre las distintas aplicaciones de una organización. A medida que las empresas adoptan múltiples herramientas y plataformas, la integración efectiva de sistemas garantiza la interoperabilidad, la eficiencia operativa y la coherencia de los datos. Una arquitectura sólida minimiza las brechas de comunicación, reduce la duplicación de datos y facilita el crecimiento de la infraestructura.

## ¿Qué?

La arquitectura de integración de sistemas es el diseño que conecta, coordina y controla diferentes aplicaciones, bases de datos y procesos dentro de una organización para que trabajen juntas de manera armónica.

### Objetivos

- **Interoperabilidad**: Permitir la comunicación entre sistemas dispares para compartir datos y funciones.
- **Eficiencia**: Optimizar los procesos eliminando redundancias y agilizando los flujos de información.
- **Escalabilidad**: Facilitar la adición de nuevos sistemas sin afectar la integridad del conjunto.
- **Resiliencia**: Garantizar la continuidad del servicio incluso ante fallos de componentes individuales.

### (Algunos) tipos de arquitecturas de integración


|Punto a punto|Bus de servicios empresariales (ESB)|Arquitectura orientada a servicios (SOA)|Arquitectura de microservicios|Arquitectura basada en eventos (EDA)|
|-|-|-|-|-|
|Conecta sistemas directamente entre sí para intercambiar datos.|Un bus de servicios centraliza el control de las comunicaciones.|Proporciona un marco modular en el que las funciones se exponen como servicios reutilizables.|Divide una aplicación en microservicios autónomos que interactúan mediante APIs.|Las aplicaciones responden a eventos publicados por otros sistemas.|
|Es simple pero tiende a volverse complejo con la adición de nuevos sistemas, generando una malla caótica.|Ofrece un punto de acceso único para todos los sistemas conectados.|Usa protocolos estandarizados como SOAP y WSDL.|Permite un desarrollo, despliegue y escalado independientes.|Usa sistemas de mensajería como Kafka o RabbitMQ para la comunicación.|
||Facilita el seguimiento, la seguridad y la gestión de servicios.|Permite la composición de servicios complejos a partir de componentes individuales.|Se apoya en contenedores para mejorar la portabilidad.|Es útil para sistemas que requieren procesamiento en tiempo real.|
||[Mule ESB](https://www.mulesoft.com/es/resources/esb/what-mule-esb) / [IBM WebSphere Message Broker](https://www.ibm.com/mx-es/topics/message-brokers)|Oracle SOA Suite / SAP NetWeaver|*Netflix* / *Amazon*|*LinkedIn* / *Uber*

### Herramientas, términos y tecnologías clave

- **Middleware**: Software que facilita la comunicación y gestión de datos entre aplicaciones, como MuleSoft o IBM WebSphere.
- **API management**: Herramientas que controlan, protegen y supervisan el uso de APIs, como Apigee o Kong.
- **Plataformas de integración como servicio (iPaaS)**: Permiten la integración en la nube sin gestión de infraestructura, como Dell Boomi o Microsoft Azure Logic Apps.

## ¿Para qué?

- **Optimización de procesos**: Reducir el tiempo de respuesta de las operaciones al permitir un intercambio rápido de datos entre sistemas.
- **Estandarización**: Aplicar estándares comunes de comunicación para simplificar la conexión de sistemas dispares.
- **Visibilidad**: Mejorar el seguimiento de datos y la detección de errores en los procesos integrados.
- **Innovación**: Facilitar la incorporación de nuevas tecnologías sin afectar la infraestructura existente.

## ¿Cómo?

1. **Evaluar requerimientos**: Analizar los sistemas existentes, las áreas de comunicación crítica y los requisitos futuros para seleccionar el tipo de arquitectura más adecuado.
2. **Definir servicios**: Identificar las funciones que deben ser compartidas entre aplicaciones como servicios o APIs.
3. **Diseñar el marco**: Crear un marco de comunicación que defina cómo se intercambiarán los datos y cómo se gestionarán las conexiones.
4. **Implementar**: Conectar las aplicaciones siguiendo el marco establecido, probando la coherencia de los datos y la compatibilidad.
5. **Monitorear**: Supervisar las conexiones para detectar errores, medir el rendimiento y asegurar el cumplimiento de los objetivos.
