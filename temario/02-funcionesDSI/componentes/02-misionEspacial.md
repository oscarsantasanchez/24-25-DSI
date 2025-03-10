# Una misión espacial - Componentes de su sistema de información

## ¿Por qué?

Las misiones espaciales enfrentan desafíos extraordinarios en la gestión de su ecosistema informacional, con implicaciones directas para su éxito, seguridad y viabilidad:

|||
|-|-|
|Entorno extremadamente hostil|Las condiciones del espacio (radiación, vacío, temperaturas extremas, microgravedad) generan amenazas constantes para la integridad de los sistemas de información, requiriendo arquitecturas con niveles excepcionales de tolerancia a fallos.|
|Latencia crítica en comunicaciones|Las enormes distancias generan retrasos significativos en la transmisión de datos (desde segundos hasta horas según la misión), impidiendo la toma de decisiones en tiempo real y requiriendo altos niveles de autonomía de los sistemas embarcados.|
|Ancho de banda limitado|Las restricciones en las comunicaciones espaciales limitan severamente la cantidad de datos que pueden transmitirse, obligando a establecer criterios rigurosos de priorización y compresión de información.|
|Imposibilidad de intervención física directa|Una vez desplegada la misión, los sistemas no pueden ser físicamente reparados o reemplazados mediante intervención humana convencional, lo que exige capacidades de autorrecuperación y redundancia.|
|Complejidad organizativa multinivel|Las misiones espaciales involucran múltiples organizaciones (agencias, contratistas, instituciones científicas, colaboradores internacionales) con diferentes objetivos, prioridades, culturas organizativas y estándares técnicos.|
|Ciclos de desarrollo extraordinariamente largos|Desde el diseño inicial hasta la conclusión, una misión espacial puede extenderse durante décadas, generando problemas de obsolescencia tecnológica y discontinuidad en los equipos humanos involucrados.|
|Necesidad de toma de decisiones bajo incertidumbre extrema|La imposibilidad de anticipar todas las condiciones y eventos posibles exige sistemas capaces de manejar situaciones completamente imprevistas con información limitada y parcial.|

## ¿Qué?

Identificar:

<div align=center>

|Hardware|Software|Datos|Procedimientos|Usuarios|
|-|-|-|-|-|

</div>

## ¿Para qué?

|||Abordando...|
|-|-|-|
|Supervivencia y continuidad operativa | Garantiza la capacidad de la misión para mantener sus funciones críticas ante fallos, eventos inesperados y condiciones adversas extremas. | • Entorno extremadamente hostil<br>• Imposibilidad de intervención física directa |
|Autonomía operacional | Permite a los sistemas embarcados tomar decisiones adecuadas durante los períodos en que la comunicación con Tierra es imposible o sujeta a retardos inaceptables. | • Latencia crítica en comunicaciones<br>• Necesidad de toma de decisiones bajo incertidumbre extrema |
|Optimización de recursos limitados | Facilita la gestión eficiente de recursos críticos y finitos como energía, propulsante, ancho de banda y capacidad computacional. | • Ancho de banda limitado<br>• Entorno extremadamente hostil |
|Coordinación interinstitucional | Posibilita la colaboración efectiva entre las múltiples organizaciones involucradas, armonizando sus diferentes objetivos, procesos y sistemas. | • Complejidad organizativa multinivel<br>• Ciclos de desarrollo extraordinariamente largos |
|Capitalización del conocimiento | Permite capturar, preservar y transferir el conocimiento acumulado a lo largo de los extensos ciclos de vida de las misiones, mitigando el impacto de los cambios en los equipos humanos. | • Ciclos de desarrollo extraordinariamente largos<br>• Complejidad organizativa multinivel |
|Adaptabilidad ante lo imprevisto | Proporciona la capacidad de reconfigurarse y adaptarse ante situaciones no contempladas en el diseño original, maximizando las posibilidades de cumplir los objetivos de la misión. | • Necesidad de toma de decisiones bajo incertidumbre extrema<br>• Imposibilidad de intervención física directa |
|Validación científica rigurosa | Garantiza la integridad, trazabilidad y confiabilidad de los datos científicos obtenidos, permitiendo su verificación y uso por la comunidad científica global. | • Ancho de banda limitado<br>• Complejidad organizativa multinivel |

## ¿Cómo?

### Empezando por lo obvio

#### Hardware

- Computadoras de vuelo con redundancia múltiple.
- Sistemas de comunicaciones (antenas, transmisores/receptores).
- Instrumentos científicos y sensores especializados.
- Dispositivos de almacenamiento de datos endurecidos contra radiación.
- Sistemas de energía (paneles solares, RTGs, baterías).
- Infraestructura terrestre (estaciones de seguimiento, centros de control).
- Equipos de soporte vital (en misiones tripuladas).

#### Software

- Sistema operativo de tiempo real para computadoras de vuelo.
- Software de control de actitud y navegación.
- Sistemas de telemetría y comando.
- Software de control de instrumentos científicos.
- Algoritmos de detección y corrección de fallos.
- Software de planificación y secuenciación de actividades.
- Sistemas de procesamiento y análisis de datos científicos.

#### Datos

- Telemetría de estado del sistema (temperaturas, voltajes, orientación).
- Datos de navegación y posicionamiento.
- Información científica recopilada por los instrumentos.
- Comandos y secuencias de operaciones.
- Modelos de referencia y parámetros de calibración.
- Registros históricos de operaciones y anomalías.
- Planificaciones y cronogramas de actividades.

#### Procedimientos

- Protocolos de lanzamiento y despliegue inicial.
- Procedimientos de operaciones nominales.
- Protocolos de respuesta a anomalías y emergencias.
- Procesos de validación y distribución de comandos.
- Procedimientos de calibración de instrumentos.
- Protocolos de comunicación entre equipos.
- Procesos de validación y distribución de datos científicos.

#### Usuarios

- Controladores de vuelo y operadores de sistemas.
- Científicos de la misión e investigadores.
- Ingenieros de sistemas y subsistemas.
- Planificadores de actividades.
- Directores y gestores de la misión.
- Astronautas o tripulación (en misiones tripuladas).
- Agencias espaciales y organizaciones colaboradoras.

### Los casos límite

<ul>
<li><details><summary>Red de Espacio Profundo (DSN)</summary>
Infraestructura de comunicaciones terrestre compartida entre múltiples misiones

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** La DSN proporciona servicios esenciales de comunicación para la misión, pero es un recurso compartido administrado independientemente que da servicio a múltiples misiones simultáneamente. La misión tiene derecho a utilizarla en períodos programados, pero no tiene control directo sobre su gestión, mantenimiento o arquitectura.
</details>
</li>
<li><details><summary>Modelos digitales gemelos</summary>
Réplicas virtuales completas de la nave utilizadas para simulación y pruebas

- ***¿Pertenece?*** Sí
- ***Justificación*** Estos modelos son creados específicamente para la misión y forman parte integral de los procesos de desarrollo, pruebas y resolución de problemas. Aunque operan en entornos separados del sistema de vuelo, son componentes oficiales del ecosistema informacional de la misión, facilitando la toma de decisiones y el diagnóstico de situaciones anómalas.
</details>
</li>
<li><details><summary>Datos de misiones anteriores utilizados como referencia</summary>
Información histórica de otras misiones que sirve como precedente

- ***¿Pertenece?*** No
- ***Justificación*** Aunque estos datos pueden ser consultados e influir en las decisiones, pertenecen a los sistemas de información de sus respectivas misiones. Son recursos externos que se utilizan como referencia pero no forman parte del sistema actual, salvo que fragmentos específicos hayan sido formalmente incorporados a la base de conocimiento oficial de la misión.
</details>
</li>
<li><details><summary>Software desarrollado por laboratorios universitarios</summary>
Programas especializados creados por instituciones académicas para instrumentos específicos

- ***¿Pertenece?*** Sí
- ***Justificación*** Una vez aceptado e integrado en el sistema operativo de la misión, este software pasa a formar parte del sistema oficial independientemente de su origen. Ha pasado por los rigurosos procesos de verificación y validación requeridos y está bajo el control de configuración de la misión, aunque su mantenimiento pueda seguir a cargo de los laboratorios que lo desarrollaron.
</details>
</li>
<li><details><summary>Datos científicos procesados por equipos externos</summary>
Información recopilada por la misión pero analizada por científicos independientes

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** Los datos brutos y los productos de nivel básico pertenecen al sistema de información de la misión. Las interpretaciones, análisis avanzados y hallazgos desarrollados posteriormente por equipos científicos externos constituyen derivaciones que, aunque basadas en información del sistema, ya no forman parte integral del mismo, a menos que sean oficialmente incorporados.
</details>
</li>
<li><details><summary>Sistemas climáticos y meteorológicos terrestres</summary>
Información sobre condiciones atmosféricas que afectan a las comunicaciones

- ***¿Pertenece?*** No
- ***Justificación*** Aunque estas condiciones afectan a la operativa de la misión, especialmente a las comunicaciones, los sistemas que recopilan y procesan esta información son completamente independientes. La misión puede consumir estos datos, pero no forman parte de su sistema de información propio.
</details>
</li>
<li><details><summary>Conocimiento implícito de ingenieros veteranos</summary>
Experiencia no documentada de personal con décadas de experiencia en misiones similares

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** El conocimiento formalizado en procedimientos, notas técnicas o decisiones documentadas forma parte del sistema. Sin embargo, la experiencia personal no capturada formalmente permanece como un recurso valioso pero externo al sistema formal de información, que solo se incorpora parcialmente cuando se manifiesta en decisiones específicas.
</details>
</li>
<li><details><summary>Sistema de navegación GPS/GNSS</summary>
Infraestructura de posicionamiento gestionada independientemente

- ***¿Pertenece?*** No
- ***Justificación*** Para misiones en órbita terrestre baja que utilizan GPS/GNSS, estos sistemas son servicios externos que la nave utiliza como referencia pero que no están bajo su control. Son sistemas independientes con sus propias arquitecturas y gestión, de los que la misión es simplemente un usuario.
</details>
</li>
<li><details><summary>Algoritmos autónomos de aprendizaje automático</summary>
Sistemas que evolucionan y ajustan sus parámetros durante la misión

- ***¿Pertenece?*** Sí
- ***Justificación*** Aunque estos sistemas pueden evolucionar de formas no totalmente predecibles, están integrados oficialmente en la arquitectura de la misión y operan dentro de límites y marcos definidos. Su capacidad de aprendizaje es una característica diseñada deliberadamente como parte del sistema de información de la misión.
</details>
</li>
<li><details><summary>Repositorios públicos de datos científicos</summary>
Plataformas que almacenan y distribuyen los hallazgos científicos tras su publicación

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** Estos repositorios contienen datos originados en la misión, pero bajo una forma procesada y con estructuras adaptadas para su uso científico general. Representan una extensión del sistema de información original, transformada para servir a objetivos de diseminación científica más amplios, funcionando como una interfaz entre el sistema de la misión y la comunidad científica.
</details>
</li>
<li><details><summary>Comunicaciones informales entre equipos</summary>
Intercambios por canales no oficiales (emails personales, mensajería instantánea)

- ***¿Pertenece?*** No
- ***Justificación*** Aunque pueden contener información relevante para la misión, estas comunicaciones no siguen los protocolos formales establecidos ni se integran en los registros oficiales. Representan un canal paralelo que, si bien puede influir en decisiones, no forma parte del sistema de información reconocido de la misión.
</details>
</li>
</ul>
