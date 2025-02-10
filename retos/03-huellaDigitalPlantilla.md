# Índice de exposición digital: propuesta de herramienta de valoración

## ¿Por qué?

En el análisis de nuestra huella digital, no todos los hallazgos tienen el mismo impacto o nivel de riesgo. Necesitamos una forma sistemática y objetiva de evaluar cada pieza de información que encontramos sobre nosotros en internet, considerando tanto su relevancia como nuestra capacidad de control sobre ella. Además, la repetición de información en múltiples fuentes puede amplificar su impacto, requiriendo una valoración que tenga en cuenta este factor multiplicador.

## ¿Qué?

La hoja de cálculo presentada aquí es una herramienta cuantitativa que permite valorar el nivel de exposición de nuestra información personal en internet. Combina tres factores clave:

- La relevancia de la información encontrada.
- Nuestro nivel de control sobre ella.
- El efecto multiplicador de las repeticiones.

## ¿Para qué?

- Priorizar qué información requiere atención más urgente.
- Cuantificar objetivamente nuestra exposición digital.
- Comparar diferentes estados de nuestra huella digital a lo largo del tiempo.
- Identificar patrones y tendencias en nuestra presencia online.
- Tomar decisiones informadas sobre la gestión de nuestra identidad digital.
- Medir el impacto de nuestras acciones de control y mitigación.

## ¿Cómo?

|![](/images/indiceExposicionDigital.png)
|:-:
|[Implementación del índice en Google Sheet](https://docs.google.com/spreadsheets/d/1pUTiEIA7C7spM6GfGkYb8MvAgWVvHBAqcLtFk_PHlog/edit?usp=sharing)

#### Cálculo del índice

La herramienta asigna pesos específicos a cada factor:

<div align=center>

|Relevancia|Control|
|-|-|
|Alta (definitivamente soy yo) = 1.0|Total (puedo modificar/eliminar) = 0.2|
|Media (probablemente soy yo) = 0.5|Parcial (puedo solicitar cambios) = 0.5|
|Baja (podría no ser yo) = 0.25|Nulo (no puedo modificar) = 1.0|
|Nula (no soy yo) = 0.1|-|

</div>

Para cada hallazgo, el índice se calcula mediante la fórmula:
```
Índice = VLOOKUP(relevancia, tabla_relevancia, 2, false) + 
         COUNTIF(rango_relevancia, relevancia_actual)*0.2
```

> Nota: la fórmula añade un 0.05 adicional por cada repetición del mismo nivel de relevancia.

Esta fórmula:

1. Obtiene el valor base según la relevancia.
1. Cuenta las ocurrencias previas del mismo nivel de relevancia.
1. Añade 0.2 por cada repetición.
1. Multiplica por el factor de control correspondiente.

#### Interpretación

- Valores cercanos a 0: Exposición baja o controlada.
- Valores medios (0.3-0.6): Exposición moderada.
- Valores altos (>0.6): Exposición significativa que requiere atención.

#### Limitaciones

- No considera el contenido específico, solo su categorización.
- La ponderación es subjetiva y puede necesitar ajustes según el contexto.
- No evalúa el impacto cualitativo de la información.
