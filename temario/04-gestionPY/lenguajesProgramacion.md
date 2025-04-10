# GdPyIS > Lenguajes de programación

|Herramientas|Diseño|Implantación|Valoración|
|-|-|-|-|
|[**Lenguajes de programación**](lenguajesProgramacion.md)|[Evaluación de requisitos y selección de sistemas](requisitos.md)|[Gestión del cambio y adopción del usuario](gestionDelCambio.md)|[Indicadores](indicadores.md)|
|[NoCode](noCode.md)|[Arquitectura de integración de sistemas](arquitectura.md)|[Gestión de la seguridad e integridad de datos](gestionSeguridad.md)|[Gestión de riesgos](riesgos.md)|
|[Metodologías de desarrollo](metodologiasDesarrollo.md)
|[Tipología de aplicaciones](tipologia.md)
|[Sistemas ERP (Enterprise Resource Planning)](erp.md)

## ¿Por qué?

La integración de sistemas requiere que los datos y las funciones fluyan sin problemas entre diferentes aplicaciones y tecnologías. Para esto, los lenguajes de programación son esenciales, ya que permiten crear soluciones que aseguren una comunicación fluida entre las partes de un sistema integrado.

La elección de un lenguaje y las herramientas adecuadas facilita la construcción, el mantenimiento y la evolución de la infraestructura tecnológica.

## ¿Qué?

Un lenguaje de programación es una forma de comunicación entre el desarrollador y el ordenador, que permite escribir instrucciones para que este último ejecute una variedad de tareas.

### Clasificaciones

#### Por nivel de abstracción

- **De bajo nivel**: Más cercanos al lenguaje máquina, incluyen el código ensamblador. Son muy rápidos, pero requieren un conocimiento profundo del hardware.
- **De alto nivel**: Más cercanos al lenguaje humano, como Python, Java, C#. Son más fáciles de aprender y utilizar, pero pueden sacrificar algo de rendimiento.
- **Intermedios**: Como C o C++, que combinan características de alto y bajo nivel.

#### Por paradigma de programación

- **Imperativos**: Siguen una secuencia ordenada de instrucciones para cambiar el estado del programa, como C, Python o Java.
- **Funcionales**: Tratan la computación como la evaluación de funciones matemáticas, evitando cambios de estado. Ejemplo: Haskell, Lisp.
- **Orientados a objetos**: Modelan datos como objetos que interactúan entre sí. Ejemplo: Java, Python, C#.
- **Lógicos**: Definen un conjunto de reglas que la computadora debe satisfacer para resolver un problema. Ejemplo: Prolog.
- **Multiparadigma**: Permiten programar en múltiples estilos, como Python y Scala.

#### Por su propósito

- **Propósito general**: Usados para desarrollar una amplia variedad de aplicaciones. Ejemplo: Java, Python, C++.
- **Dominio específico**: Diseñados para un tipo particular de aplicaciones, como SQL para bases de datos o MATLAB para cálculos matemáticos.

#### Por su compilación e interpretación

- **Compilados**: El código fuente se traduce a código máquina antes de ejecutarse, como en C++ o Go.
- **Interpretados**: El código fuente se traduce y ejecuta línea por línea durante la ejecución, como en Python o JavaScript.

### Lenguajes de programación más populares para la integración (2024-2025)

- **Python**: Lidera la integración de datos, automatización, IA y análisis. Destaca en ETL, orquestación de sistemas heterogéneos y procesamiento de datos a gran escala.
- **Java**: Mantiene posición dominante en entornos empresariales grandes. Ofrece estabilidad, portabilidad y amplio ecosistema para APIs, microservicios y procesamiento backend.
- **JavaScript/TypeScript**: Fundamentales para integraciones web y APIs. TypeScript añade tipado fuerte, mejorando la mantenibilidad en proyectos complejos de integración.
- **C#/.NET**: Esencial en ecosistemas Microsoft con creciente adopción multiplataforma. Óptimo para integraciones empresariales y sistemas Windows.
- **Go**: Notable para microservicios, herramientas DevOps e integraciones de alto rendimiento con baja huella de memoria.
- **Rust**: Emergente para integraciones que requieren alto rendimiento, concurrencia segura y proximidad al hardware.
- **Kotlin**: Alternativa moderna para ecosistemas Java, especialmente en integraciones Android-Backend.

### Frameworks y herramientas de integración relevantes (2024-2025)

#### Frameworks generales

- **Spring Boot/Spring Cloud (Java)**: Ecosistema completo para microservicios, integraciones cloud-native y arquitecturas reactivas.
- **FastAPI y Django (Python)**: FastAPI para APIs de alto rendimiento y Django para sistemas web completos con administración integrada.
- **NestJS y Express (Node.js)**: NestJS para integraciones empresariales estructuradas y Express para soluciones ligeras.
- **ASP.NET Core (C#)**: Framework moderno para web, APIs y microservicios con optimizaciones cloud-native.
- **gRPC**: Comunicación eficiente entre servicios mediante protocolos binarios, independiente del lenguaje.

#### Frameworks específicos para integración

- **Apache Camel**: Framework especializado para patrones de integración empresarial (EIP).
- **Dapr**: Plataforma agnóstica de lenguaje para construir aplicaciones distribuidas y microservicios.
- **MuleSoft Anypoint**: Plataforma iPaaS (Integration Platform as a Service) para orquestación de APIs.
- **Apache Kafka/Kafka Streams**: Para arquitecturas de integración basadas en eventos y procesamiento de streams.
- **Apache Airflow**: Orquestación de flujos de trabajo para integraciones complejas.

## ¿Para qué?

- **Flujo de datos**: Los lenguajes y frameworks seleccionados facilitan el procesamiento de datos entre sistemas.
- **Automatización**: Crear soluciones que automaticen tareas repetitivas.
- **Interoperabilidad**: Desarrollar conexiones a través de APIs para compartir información entre aplicaciones dispares.
- **Escalabilidad**: Diseñar sistemas capaces de crecer con la organización.

### Consideraciones por perfil profesional

En el contexto de la integración de sistemas, las decisiones sobre lenguajes de programación tienen diferentes implicaciones según el perfil profesional:

|||
|-|-|
|Integración entre sistemas SCADA y ERP mediante interfaces programadas | Evaluación de costes de desarrollo vs. adquisición de soluciones comerciales|
|Lenguajes para automatización industrial (PLC, Python para IoT, etc.) | Impacto en tiempo de mercado (time-to-market) según la elección tecnológica|
|Sistemas de ejecución de manufactura (MES) y su programación | Gestión de dependencias con proveedores tecnológicos|
|Desarrollo de gemelos digitales mediante lenguajes de simulación | ROI de diferentes aproximaciones de desarrollo e integración|
|Programación para análisis de datos en mantenimiento predictivo | Criterios no técnicos para evaluación de propuestas de desarrollo|
|Sistemas embebidos en maquinaria y su comunicación con sistemas corporativos | Estrategias de contratación y gestión de talento técnico|
|Interfaces entre sistemas de control de calidad y sistemas de gestión | Elaboración de RFPs (Request for Proposal) para proyectos de integración|
|Programación para trazabilidad en cadenas de suministro | Cumplimiento normativo y auditoría de sistemas integrados|

## ¿Cómo?

1. **Selección del lenguaje**: Identificar las necesidades del proyecto (compatibilidad, rendimiento, facilidad de uso).
2. **Identificar frameworks**: Elegir frameworks que ofrezcan las bibliotecas necesarias para el tipo de integración requerida.
3. **Desarrollo**: Implementar interfaces que permitan el intercambio de datos, crear controladores para los servicios y manejar errores.
4. **Pruebas**: Asegurar la integridad de los datos y la interoperabilidad de las aplicaciones a través de pruebas unitarias e integrales.
5. **Documentación**: Documentar el código, APIs, y procesos para el mantenimiento futuro.
