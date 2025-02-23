# Caso de estudio: falla del proyecto de ERP en Hershey Foods

## Contexto

En 1999, Hershey Foods, la conocida compañía de chocolates, decidió implementar un sistema integrado de planificación de recursos empresariales (ERP), junto con sistemas de gestión de la cadena de suministro (SCM) y de relación con el cliente (CRM). Esta implementación se planeó para modernizar y optimizar las operaciones de la empresa.

## Implementación

Hershey escogió SAP para el ERP, Siebel para el CRM, y Manugistics para el SCM, planificando su implementación en un plazo agresivamente corto de 30 meses. Además, decidieron llevar a cabo la implementación en un periodo crítico: justo antes de la temporada de Halloween y Navidad, dos de los momentos de mayor demanda para la empresa.

## Problemas

<div align=center>

|||
|-|-|
|Sobreestimación de capacidades|Hershey subestimó la complejidad de coordinar tres sistemas distintos en un mismo proceso de implementación.
|Gestión de cambios deficiente|No hubo una adecuada preparación ni formación para los empleados sobre los nuevos sistemas, lo que llevó a una adopción problemática.
|Tiempo de implementación no realista|El plazo para la implementación fue demasiado corto para un proyecto de esta envergadura, especialmente considerando que se hizo durante el periodo de alta demanda.

</div>

## Consecuencias

<div align=center>

|||
|-|-|
|Interrupciones en la cadena de suministro|La incapacidad para procesar órdenes a tiempo resultó en una severa interrupción de la cadena de suministro. Hershey fue incapaz de entregar $100 millones en productos para Halloween de 1999.
|Impacto financiero|La compañía sufrió una caída del 19% en sus beneficios en el tercer trimestre de 1999 comparado con el año anterior.
|Caída en el precio de las acciones|Las acciones de Hershey cayeron aproximadamente un 8% en 1999, reflejando la pérdida de confianza de los inversores.

</div>

## Lecciones

<div align=center>

|Antipatrón|Relación
|-|-|
|Ausencia de métricas|No se establecieron KPIs claros para monitorear la integración de los sistemas ERP, SCM y CRM. Esto complicó el seguimiento del progreso y la identificación temprana de problemas. |
|Ignorancia de restricciones|Implementación simultánea de tres sistemas complejos en un plazo corto sin considerar las limitaciones técnicas y de tiempo, subestimando la complejidad del proyecto. |
|Optimismo injustificado|Se procedió con un cronograma agresivo basado en un optimismo infundado sobre la capacidad de la empresa para manejar grandes cambios durante la temporada de mayor venta. |
|Falta de control|No se definieron hitos claros ni se implementaron planes de contingencia efectivos, lo que dificultó la gestión del proyecto ante imprevistos. |
|Análisis superficial de riesgos|Falta de un análisis detallado de riesgos asociados con la implementación simultánea de los sistemas, sin evaluar adecuadamente las consecuencias de posibles retrasos o fallos técnicos. |
|Obsesión por el consenso|Aunque menos documentado, en contextos similares, la dilación o suavización de decisiones críticas para mantener el consenso puede impedir acciones decisivas necesarias para ajustar el rumbo. |

</div>