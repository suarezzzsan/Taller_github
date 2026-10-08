
 <div align="center">
  
# Apache Arrow
### Proyecto realizado por un científico de datos
#### Zahra Suarez, Juan Galeano, David Marroquín

</div>

## Wes Mckinney
**Creador de la librería Pandas en Python**

FOTO 1

Wes Mckinney nació en 1985 en Estados Unidos. Es un emprendedor e ingeniero especializado en herramientas para desarrolladores de IA y sistemas de datos. Es fundador en Kenn Software. También es arquitecto principal de Posit, donde contribuyó a la estrategia de Python e IA. Es fundador de Voltron Data, Usar Labs y Datapad. Desde 2008, lleva desarrollando proyectos de software. Actualmente, la mayor parte de su trabajo se implementa a través de Kenn Software:agentsview para la búsqueda de sesiones y el análisis de tokens en agentes de codificación. 

FOTO 1
Imagen Wes Mckinney

## Contexto y problema del Proyecto

A la hora de analizar datos de forma masiva(Big Data), las organizaciones y científicos de datos utilizan varias herramientas y lenguajes en un mismo flujo de trabajo, cada herramienta utiliza su propio formato interno para representar tablas y data frames. Para conectar estas herramientas distintas entre sí, se requerían conversores individuales. El problema surge ya que, transferir datos entre diferentes plataformas o lenguajes, requería traducir y copiar continuamente los bloques de datos en memoria, lo que era un desperdicio de tiempo y rendimiento.


## Solución del problema
Apache Arrow se diseñó para resolver esta fragmentación estableciendo una memoria columnar estándar y abierta. Al lograr esto, se permitía que múltiples procesos y lenguajes compartan el mismo bloque de memoria sin duplicar ni traducir datos, lo que lo hacía más óptimo, y ahorraba tiempo, a esto se le conoce como zero-copy. Finalmente, Apache Arrow, facilita la creación de librerías y motores de cálculo reutilizables que combina diferentes herramientas como Python,R, Java entre otros.

FOTO 2
Imagen de apache arrow

## Estructura y tipo de datos utilizados
- A diferencia de las estructuras organizadas por filas, arrow organiza los datos por columnas continuas en memoria.
- Está diseñado para datos tabulares analíticos(Data Frames y tablas)
  - Soporta arreglos multidimensionales
  - Datos anidados
  - Cadenas de texto
  - Mapas de bits para valores nulos

#### Ejemplo 
  
| Tipo | Código | Color |
|---|---|---|
| A | 1 | "Blanco".  |
| B | 2 | "Amarillo" |
| C | 6 | "Rojo"     |


Al almacenar los datos por columnas continuas, reduce fallos de caché en CPU y GPU, optimizando el procesamiento de datos y permitiendo algoritmos de comprensión especializada


## Casos de uso avanzados e integraciones en la industria
**Integración con**
- NVIDIA
- Anaconda
- MapD

## Frase de cierre
>Dada lo difícil que es desarrollar software libre, entre más podamos desfragmentar el ecosistema y trabajar juntos para construir librerías reutilizables y sistemas portables, todos seremos mucho más productivos y exitosos.” (traducido del inglés al español con traductor de google) -  Wes Mckinney

### ***Referencias***

1. Wes McKinney. (s. f.). *Wes McKinney*. https://wesmckinney.com/
2. Apache Arrow: A Cross-language Development Platform for In-memory Data – Wes McKinney. (2018, 11 julio). *Wes McKinney*. https://wesmckinney.com/transcripts/2018-07-11-scipy-apache-arrow-development-platform
