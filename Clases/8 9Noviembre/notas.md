# Clase 7
## Reducción de dimensionalidad
- ¿Por qué es importante reducir la dimensionalidad de un conjunto de datos al construir un modelo de aprendizaje automático?
    - La dimensionalidad es un problema de poder computacional
    - Es importante realizar un análisis 
    - Si hay variables fuertemente relacionadas va a meter ruido al modelo
- **Selección de atributos**: Seleccionamos aquellos atributos que van a aportar información relevante y descartamos los redundantes o poco útiles
    - Ayuda a reducir el coste espacial y computacional al desarrollar un modelo
    - Se escogen los mejores atributos
- **Extracción de atributos**: Calcula nuevos atributos a partir de atributos ya existentes para resumir mejor su información 
- La clasificación de atributos se clasifica en dos grandes tipos:
    - **Algorítmos Filtro**:
    - Evaluan los algorítmos de forma independiente al clasificador que se utilizará más adelante
    - Analiza los atributos relevantes utilizando criterio propio
    - **Algorítmos empotrados**: 
    - Utilizan al clasificador que se empleará posteriormente
    - Evalúa que atributos o subconjuntos son los más adecuado
    - Puede causar sobreaprendizaje(overfitting) 
- Existen dos grandes grupos de métodos
    1. Algorítmos univerantes
    - Métodos que evaluan los atributos individualmente
    - Analiza cada característica individualmente para entender que tan relevante es
    - **Selección de máxima relevancia**

- **Análisis Componentes Principales (PCA)**
- Se basa en la matriz de covarianzas o correlaciones de los datos originales
- [Evaluación análisis componentes principales](https://chatgpt.com/share/6af24dd5-d67c-83eb-885d-20b7c18f560d)
- [Notebook revisado en clase](https://colab.research.google.com/github/andres-merino/AprendizajeAutomaticoInicial-05-N0105/blob/main/2-Notebooks/06-1-Reduccion-Dimensionalidad.ipynb#scrollTo=dd629901)

---
## Materiales de clase
- [Tutor de CHATGPT](https://chatgpt.com/g/g-674f787b286c8191aee6a93bde4ede57-tutor-aa-seleccion-de-atributos)
- [Conversación con ChatGPT](https://chatgpt.com/share/6af24bd5-793c-83eb-8b4d-e31ff40fcd86)