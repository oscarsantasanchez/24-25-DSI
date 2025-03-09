# La universidad - Componentes de su sistema de información

## ¿Por qué?

Las instituciones en general y las universitarias en particular enfrentan desafíos significativos en la gestión de su información y recursos tecnológicos:

|||
|-|-|
|Complejidad organizativa|Las universidades operan como ecosistemas complejos con múltiples departamentos, facultades y servicios que generan y consumen grandes volúmenes de información heterogénea, creando silos aislados de datos difíciles de integrar.|
|Fronteras difusas|Resulta problemático determinar dónde comienzan y terminan las responsabilidades institucionales en un entorno digital cada vez más híbrido, con recursos propios y externos interconectados.|
|Vulnerabilidades de seguridad|La indefinición del perímetro tecnológico institucional expone a riesgos de seguridad, con posibles brechas en la protección de datos académicos y personales sensibles.|
|Ineficiencia en inversiones|Sin una clara delimitación de qué constituye el sistema institucional, se producen duplicidades, gastos innecesarios y descuido de componentes críticos para la misión universitaria.|
|Incumplimiento normativo|La ambigüedad sobre qué datos y sistemas están bajo control institucional complica el cumplimiento de normativas como RGPD, dificultando determinar responsabilidades sobre tratamiento de información.|
|Discontinuidad de servicios|La falta de identificación de componentes críticos impide establecer adecuados planes de contingencia, generando vulnerabilidad ante incidentes tecnológicos.|
|Barreras a la innovación|La ausencia de una visión integral del sistema dificulta la planificación estratégica tecnológica y la evolución coherente de la infraestructura digital universitaria.|

## ¿Qué?

Identificar:

<div align=center>

|Hardware|Software|Datos|Procedimientos|Usuarios|
|-|-|-|-|-|

</div>

## ¿Para qué?

|||Abordando...|
|----------|-------------|--------------------------------|
|Seguridad y responsabilidad legal | Definir qué elementos pertenecen al SI determina el perímetro de seguridad que debe protegerse y establece las responsabilidades legales sobre datos personales, propiedad intelectual y cumplimiento normativo. | • Vulnerabilidades de seguridad<br>• Fronteras difusas<br>• Incumplimiento normativo |
|Planificación de recursos | Permite identificar correctamente dónde invertir presupuesto, personal y esfuerzos de mantenimiento, evitando destinar recursos a elementos que no son responsabilidad institucional. | • Ineficiencia en inversiones<br>• Complejidad organizativa<br>• Barreras a la innovación |
|Gestión de riesgos | Facilita identificar vulnerabilidades y amenazas potenciales en los componentes del sistema, permitiendo implementar controles adecuados donde realmente corresponde. | • Vulnerabilidades de seguridad<br>• Discontinuidad de servicios |
|Continuidad operativa | Ayuda a establecer protocolos de respaldo, recuperación y planes de contingencia para los componentes esenciales para el funcionamiento universitario. | • Discontinuidad de servicios<br>• Complejidad organizativa |
|Gobernanza de datos | Clarifica quién tiene autoridad sobre qué información, cómo debe gestionarse cada tipo de dato y qué políticas aplican en cada caso. | • Complejidad organizativa<br>• Incumplimiento normativo<br>• Fronteras difusas |
|Interoperabilidad y arquitectura tecnológica | Define qué sistemas deben comunicarse entre sí y cómo se estructuran las relaciones entre componentes internos y externos. | • Fronteras difusas<br>• Complejidad organizativa<br>• Barreras a la innovación |
|Auditoría y cumplimiento | Permite establecer alcances claros para auditorías de sistemas, certificaciones y evaluaciones de conformidad. | • Incumplimiento normativo<br>• Vulnerabilidades de seguridad |

## ¿Cómo?

### Empezando por lo obvio

#### Hardware

- Servidores para almacenar bases de datos académicas y administrativas
- Ordenadores en aulas, laboratorios, bibliotecas y oficinas administrativas
- Equipos de redes y comunicación (routers, switches, puntos de acceso WiFi)
- Escáneres, fotocopiadoras e impresoras
- Sistemas de seguridad física (cámaras, controles de acceso)
- Proyectores y equipamiento audiovisual para aulas
- Dispositivos de almacenamiento para copias de seguridad

#### Software

- GUIAA: sistema de gestión académica (matrícula, calificaciones, expedientes)
- PANAL + Campus: plataforma de aprendizaje virtual (LMS como Moodle, Canvas, Blackboard)
- GUIAA: Software administrativo (gestión financiera, recursos humanos, inventario)
- Koha-Kobli: Sistema de gestión bibliotecaria
- Software de correo institucional y comunicaciones
- Herramientas ofimáticas y software especializado por disciplinas
- Sistemas operativos para servidores y equipos de usuario

#### Datos

- Expedientes académicos de estudiantes
- Información del personal docente y administrativo
- Planes de estudio y contenidos académicos
- Datos de investigación y publicaciones
- Información financiera y presupuestaria
- Registros de biblioteca (catálogo, préstamos)
- Estadísticas institucionales y reportes

#### Procedimientos

- Procesos de admisión y matrícula
- Protocolos para evaluación y calificación
- Procedimientos administrativos (contratación, compras)
- Políticas de seguridad de la información
- Protocolos de respaldo y recuperación de datos
- Procedimientos de atención al estudiante
- Normativas académicas y reglamentos

#### Usuarios

- Estudiantes
- Personal docente e investigador
- Personal administrativo y de servicios
- Directivos y gestores universitarios
- Egresados
- Candidatos y aspirantes
- Entidades colaboradoras (empresas de prácticas, socios de investigación)

### Los casos límite

<ul>
<li><details><summary>Portátil personal de un profesor con software institucional</summary>
El dispositivo es privado pero contiene elementos (software, datos) institucionales y se usa para funciones oficiales

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** No forma parte del hardware del SI, pero el software institucional y los datos académicos que contiene sí pertenecen al SI. Existe una responsabilidad compartida donde la universidad gestiona las aplicaciones pero no el dispositivo.
</details>
</li>
<li><details><summary>Servicios cloud (Microsoft 365, Google Workspace)</summary>
La infraestructura física pertenece a un proveedor externo pero está contratada y configurada específicamente para la universidad

- ***¿Pertenece?*** Sí
- ***Justificación*** Aunque la infraestructura física no es propiedad de la universidad, estos servicios son gestionados, configurados y administrados por la institución mediante contratos que establecen responsabilidades sobre los datos. Son extensiones virtuales del SI universitario.
</details>
</li>
<li><details><summary>Base de datos de la cafetería universitaria (empresa externa)</summary>
Procesa datos de la comunidad pero es gestionada por un concesionario independiente

- ***¿Pertenece?*** No
- ***Justificación*** No está bajo el control administrativo de la universidad ni tiene como propósito principal servir a la misión educativa. Es un sistema paralelo que interactúa con la comunidad universitaria pero no forma parte integral del SI institucional.
</details>
</li>
<li><details><summary>Cuentas institucionales en redes sociales</summary>
La plataforma es externa pero el contenido es oficial y gestionado por la universidad

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** El contenido y la gestión de las cuentas pertenecen al SI como parte de los datos institucionales, pero la plataforma en sí misma no. Representan un punto de conexión entre el SI y sistemas externos.
</details>
</li>
<li><details><summary>Sensores IoT en el campus (temperatura, cámaras)</summary>
Recopilan datos del entorno universitario pero no procesan información académica directamente

- ***¿Pertenece?*** Sí
- ***Justificación*** Forman parte de la infraestructura tecnológica planificada por la institución y sus datos se utilizan para la gestión del campus. Aunque no procesan información académica, contribuyen a la gestión administrativa del espacio físico universitario.
</details>
</li>
<li><details><summary>App no oficial de horarios creada por estudiantes</summary>
Utiliza datos universitarios pero sin autorización formal ni control institucional

- ***¿Pertenece?*** No
- ***Justificación*** No está bajo la gestión, control o responsabilidad de la universidad. Aunque utiliza datos universitarios, lo hace sin integración oficial en los procesos institucionales y potencialmente sin cumplir con las políticas de seguridad establecidas.
</details>
</li>
<li><details><summary>Bases de datos académicas por suscripción (JSTOR, ScienceDirect)</summary>
La universidad paga por acceso pero no controla la plataforma

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** El contenido al que se accede forma parte de los recursos de información universitarios, pero la infraestructura y gestión son externas. Son recursos contratados que extienden las capacidades del SI pero no están completamente integrados en él.
</details>
</li>
<li><details><summary>Supercomputador compartido entre varias universidades</summary>
Los recursos son compartidos entre múltiples instituciones

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** Pertenece proporcionalmente según los acuerdos de uso y propiedad establecidos. Representa un caso de SI distribuido donde la propiedad, gestión y responsabilidad se comparten mediante acuerdos interinstitucionales formales.
</details>
</li>
<li><details><summary>Carné universitario integrado con transporte público</summary>
Un dispositivo único sirve para múltiples sistemas

- ***¿Pertenece?*** Parcialmente
- ***Justificación*** La funcionalidad universitaria (identificación, acceso a servicios académicos) pertenece al SI, mientras que la funcionalidad de transporte pertenece a otro sistema. Es un elemento híbrido con componentes en múltiples sistemas de información.
</details>
</li>
<li><details><summary>Información de egresados en LinkedIn</summary>
Datos relevantes para la universidad pero en plataformas externas fuera de su control

- ***¿Pertenece?*** No
- ***Justificación*** Aunque contiene información sobre la comunidad universitaria, no está bajo el control, gestión o responsabilidad de la institución. La universidad puede interactuar con estos datos pero no forman parte de su SI oficial.
</details>
</li>
<li><details><summary>Móvil de un alumno conectado a la WiFi universitaria</summary>
El dispositivo es personal pero se conecta a infraestructura universitaria

- ***¿Pertenece?*** No
- ***Justificación*** No está gestionado por la universidad ni sirve principalmente a propósitos institucionales. La conexión WiFi sí forma parte del SI universitario, pero el dispositivo que la utiliza mantiene su autonomía y queda fuera del perímetro del sistema institucional.
</details>
</li>
</ul>
