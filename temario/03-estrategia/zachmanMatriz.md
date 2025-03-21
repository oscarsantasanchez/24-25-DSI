# Matriz Zachman

<div align=center>

||Las preguntas consideradas como primitivas dentro de la comunicación: ¿Qué?, ¿Cómo?, ¿Cuándo?, ¿Quién?, ¿Dónde? y ¿Por qué? Estas representan las dimensiones o abstracciones fundamentales necesarias para describir completamente cualquier sistema complejo. Cada columna captura un aspecto esencial del sistema, proporcionando diferentes perspectivas que, en conjunto, ofrecen una visión integral de la arquitectura empresarial.|
|-|-|
|Diferentes niveles de transformación desde la idea abstracta hasta la implementación concreta (cosificación). Cada fila corresponde a una perspectiva específica de stakeholder, desde la visión ejecutiva en el nivel contextual, pasando por la visión de negocio, la visión arquitectónica, la visión técnica, hasta llegar a los componentes detallados de implementación. Este eje vertical muestra la progresiva materialización de los conceptos, añadiendo restricciones y detalles en cada nivel, asegurando así la alineación entre la estrategia organizacional y su ejecución técnica.|La intersección de cada fila y columna genera una celda única que proporciona una representación específica del sistema desde una perspectiva particular y enfocada en una dimensión concreta, permitiendo documentar la complejidad del sistema de manera estructurada y coherente.|

</div>

||Por qué|Cómo|Qué|Quién|Dónde|Cuándo|
|-|:-:|:-:|:-:|:-:|:-:|:-:|
|**Contextual**|Lista de Objetivos|Lista de Procesos|Lista de Materiales|Lista de Unidades y Roles Organizacionales|Lista de Ubicaciones Geográficas|Lista de Eventos|
|**Conceptual**|Relación de Objetivos|Modelo de Procesos|Modelo de Relación de Entidades|Modelo de Relación de Unidades y Roles Organizacionales|Modelo de Ubicaciones|Modelo de Eventos|
|**Lógico**|Diagrama de Reglas|Diagrama de Procesos|Diagrama de Modelo de Datos|Diagrama de Relación de Roles|Diagrama de Ubicaciones|Diagrama de Eventos|
|**Físico**|Especificación de Reglas|Especificación de Funciones de Proceso|Especificación de Entidades de Datos|Especificación de Roles|Especificación de Ubicación|Especificación de Eventos|
|**Detallado**|Detalles de Reglas|Detalles de Procesos|Detalles de Datos|Detalles de Roles|Detalles de Ubicación|Detalles de Eventos|

Los principios fundamentales que guían la aplicación del Framework de Zachman incluyen los siguientes aspectos:

1. Un sistema completo que puede ser modelado por representación de las respuestas a las siguientes preguntas: ¿Por qué, quién, qué, cómo, dónde y cuándo?
1. Los seis puntos de vista de captura de todos los modelos críticos para el desarrollo del sistema.
1. Las restricciones para cada perspectiva son aditivos; las de una fila inferior se suman a los de las filas de arriba para ofrecer un creciente número de restricciones.
1. Las columnas representan abstracciones diferentes en un esfuerzo por reducir la complejidad de un modelo único que se construyen.
1. Las columnas no tienen ningún orden.
1. El modelo de cada columna debe ser único.
1. Cada fila representa una perspectiva única.
1. Cada celda es única.
1. La lógica inherente es recursiva.

## Detallado

|**Perspectiva**|**Por qué**<br>(Motivación)<br>Razones y objetivos que impulsan el sistema|**Cómo**<br>(Función)<br>Procesos y operaciones que ejecuta el sistema|**Qué**<br>(Datos)<br>Información y entidades con las que opera el sistema|**Quién**<br>(Personas)<br>Roles e individuos que interactúan con el sistema|**Dónde**<br>(Redes)<br>Ubicaciones y conexiones donde opera el sistema|**Cuándo**<br>(Tiempo)<br>Eventos y ciclos temporales del sistema|
|-|:-:|:-:|:-:|:-:|:-:|:-:|
|**Contextual**<br>(Vista del planificador/alcance)<br>Define el contexto, propósito y alcance general del sistema|Lista de Objetivos|Lista de Procesos|Lista de Materiales|Lista de Unidades y Roles Organizacionales|Lista de Ubicaciones Geográficas|Lista de Eventos|
|**Conceptual**<br>(Modelo del negocio)<br>Representa el modelo de negocio y las relaciones entre sus componentes|Relación de Objetivos|Modelo de Procesos|Modelo de Relación de Entidades|Modelo de Relación de Unidades y Roles Organizacionales|Modelo de Ubicaciones|Modelo de Eventos|
|**Lógico**<br>(Modelo del sistema)<br>Describe cómo el sistema funciona de forma independiente de la tecnología|Diagrama de Reglas|Diagrama de Procesos|Diagrama de Modelo de Datos|Diagrama de Relación de Roles|Diagrama de Ubicaciones|Diagrama de Eventos|
|**Físico**<br>(Modelo tecnológico)<br>Considera las limitaciones de la tecnología, herramientas, materiales y personas|Especificación de Reglas|Especificación de Funciones de Proceso|Especificación de Entidades de Datos|Especificación de Roles|Especificación de Ubicación|Especificación de Eventos|
|**Detallado**<br>(Componentes)<br>Especifica los componentes individuales y su implementación fuera de contexto|Detalles de Reglas|Detalles de Procesos|Detalles de Datos|Detalles de Roles|Detalles de Ubicación|Detalles de Eventos|
