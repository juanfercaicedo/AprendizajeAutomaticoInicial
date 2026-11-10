# Clase 8
## Aprendizaje no supervisado
- Conjunto de técnicas que tratan de inferir modelos a partir de datos de los cuales no conocemos la salida(resultado)
- Utiliza patrones
- Ayuda a segmentar o separar un conjunto de datos a partir de sus características
- Existen dos algorítmos:
1. **Clustering o Agrupamiento**
    - Agrupa los conjuntos dependiendo sus características
    - Si son datos que no se parecen van a estar separados en diferentes grupos/segmentos
2. **Reducción de la dimensionalidad**
    - La dimensionalidad es el conjunto de variables que tiene de datos
    - Las características son atributos que son columnas, puede añadir información inservible que disminuye el rendimiento
    - La reducción de dimensionalidad consiste en reducir las cantidades de columnas o en atributos en función de que tanto va a aportar al modelo
    - Construir características informativas y poco redundantes
---
## Tipos de agrupamientos
- Generar una función de mi conjunto de datos en un conjunto de etiquetas
- **Exclusivo**: Va a coger cada dato y nos va a dar como resultado en que grupo debe de estar, si pertenecemos a un grupo no pertenecemos a ninguno otro.
- **No exclusivo**: Nos da como resultado un vector en donde nos dice que tanto pertenece a cada grupo, por ejemplo si tenemos tres grupos, F(x0) = (0, 0.7, 0.3), no pertenece al grupo 1(0), pertenece parcialmente al grupo(0.7), pertenece parcialmente al grupo(0.3)
    - Permite pertenecer a más de un grupo
- Se puede hacer un árbol de agrupamientos
--- 
- Alusinación en un modelo, se inventa algo
- Mientras más datos tenga y más grande sea el modelo es menos probable que las cosas sean inventadas
- Los modelos funcionan prediciendo lo siguiente es decir, si tenemos una oración ocupa las palabras anteriores para predecir lo siguiente
---
## Análisis notebook
- Cuando vamos a hacer agrupamiento debemos tener cuidado con el escalado y las transformaciones
- Hay que tener cuidado con transformaciones que se apliquen como normalizado, min max scaler concentra muchos los datos
- Lo mejor es dejar los datos normales o aplican un standard scaler

---
## Materiales de clase
- [Clase 07](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase07.pdf)
- [Herramienta de IA](https://consensus.app)
- [Notebook revisado en clase](https://colab.research.google.com/github/andres-merino/AprendizajeAutomaticoInicial-05-N0105/blob/main/2-Notebooks/07-Normalizacion-Agrupamiento.ipynb)

