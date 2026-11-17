# Simulador de integración múltiple

Recurso educativo digital para la **Fase 3** del curso **Cálculo Multivariado (203057)** de la
Universidad Nacional Abierta y a Distancia (UNAD). El estudiante escribe la función, la región, el
sistema de coordenadas y los límites; el simulador **comprueba** lo que escribió. No resuelve la
integral: ese es el trabajo de la actividad 3.

## Qué hace cada módulo

| Módulo | Apoya | Qué hace |
|---|---|---|
| 1 · Región de integración | Actividad 1, ítems I y II | Representa la región en coordenadas cartesianas a partir de las desigualdades que escribe el estudiante, y contrasta su lectura de la geometría con las simetrías que la región realmente tiene. |
| 2 · Cambio de coordenadas y límites | Actividad 2, ítems I, II y III | Muestra la transformación y el jacobiano, arma la integral planteada sin resolverla y **comprueba que los límites escritos describan exactamente la misma región**. |
| 3 · Comprobación del resultado | Actividad 3, ítems I y III | Contrasta la integral, el volumen y el valor medio que el estudiante calculó a mano, sin revelar los valores correctos, y detecta si sus tres cifras son incoherentes entre sí. |
| 4 · Contraste antes y después | Actividad 4 | Enfrenta la región física en cartesianas con la región de límites sencillos en el espacio de parámetros. |

La comprobación de los límites es exacta y en dos direcciones: invierte la transformación para
verificar que ningún punto de la región quede fuera de los límites, y genera puntos a partir de los
límites para verificar que ninguno caiga fuera de la región.

Cada módulo trae un ejemplo resuelto plegado, que permanece oculto hasta que el estudiante lo abre.
El trabajo se conserva en el navegador y puede trasladarse a otro equipo mediante un código, de modo
que la fase puede desarrollarse en varias sesiones y en el orden que el estudiante decida.

## Uso

Abra `index.html` en cualquier navegador moderno. **No requiere instalación, servidor ni conexión a
internet**: mathjs, Plotly y MathJax están incluidos en `vendor/`, de manera que el recurso seguirá
funcionando aunque esos servicios cambien de dirección o el estudiante trabaje sin conectividad,
condición frecuente en las zonas rurales del Caribe colombiano en las que se sitúa el curso.

## Sistemas de coordenadas admitidos

| Sistema | Tipo | Transformación | Jacobiano |
|---|---|---|---|
| Cartesianas | doble y triple | identidad | 1 |
| Polares | doble | x = r cos θ, y = r sen θ | r |
| Cilíndricas | triple | x = r cos θ, y = r sen θ, z = z | r |
| Esféricas | triple | x = ρ sen φ cos θ, y = ρ sen φ sen θ, z = ρ cos φ | ρ² sen φ |

Los límites de cada variable pueden depender de las variables exteriores.

## Dónde está publicado

| | |
|---|---|
| Simulador | https://calculo-multivariado-203057.github.io/simulador-integracion/ |

El sitio se sirve con GitHub Pages desde la rama `main`, carpeta raíz. El archivo `.nojekyll` evita
el procesamiento de Jekyll, de modo que los archivos se publican tal como están.

## Autoría y filiación

**Pablo Emilio Gutiérrez Duncan**
Director del curso Cálculo Multivariado (203057)
Escuela de Ciencias Básicas, Tecnología e Ingeniería (ECBTI)
Universidad Nacional Abierta y a Distancia (UNAD) — CCAV Puerto Colombia, Zona Caribe
ORCID: https://orcid.org/0009-0001-6596-8536

## Cómo citar

Gutiérrez Duncan, P. E. (2026). *Simulador de integración múltiple* (versión 1.0) [Software].
Universidad Nacional Abierta y a Distancia.
https://github.com/calculo-multivariado-203057/simulador-integracion

El archivo `CITATION.cff` permite que GitHub genere la cita automáticamente y que Zenodo la lea si
se le asigna un DOI.

## Recurso relacionado

[Simulador de gradiente y optimización](https://github.com/calculo-multivariado-203057/simulador-gradiente),
para la Fase 2 del mismo curso.

## Licencia

El simulador se publica bajo **Creative Commons Atribución-NoComercial-CompartirIgual 4.0
Internacional (CC BY-NC-SA 4.0)**; véase [`LICENSE`](LICENSE).

Las bibliotecas incluidas en `vendor/` conservan sus propias licencias, que se distribuyen junto a
cada archivo:

| Componente | Versión | Licencia |
|---|---|---|
| mathjs | 12.4.2 | Apache-2.0 |
| Plotly.js | 2.32.0 | MIT |
| MathJax (salida SVG) | 3.2.2 | Apache-2.0 |
