# Clase 12
## Introducción a redes neuronales
- Una nuerona biológica reibe señales mediante sinapsis
- En redes nueronales computacionales:
  - Entrada, Nuerona(operación matemática), Activación(Función lineal o no lineal) y Salida
- Una función con parámetros, es decir dependerá de valores
  - Debe representar la transformación de una entrada x porqué esta generando una salida y
  - Siempre debe haber una función de pérdida
    - Siempre tratamos de minimizar, encontrar un valor mínimo para esa pérdida
## Modelos con una neurona o más
- La conexión de dos neuronas es la composición de dos funciones(f2(f1(x)))
- Conectar neuronas no complejiza la función que se quiere modelar
- La idea es activar las neuronas con funciones no lineales
  - Hay diferentes formas de activar las no linealidades / complejizar el modelo 
  - Las diferentes activaciones son:
    - Idendidad: Suele usarse para modelos de regresión / modelos lineales
    - Escalón: Salida binaria del perceptón clásico
      - Ej: Si recibo un valor positivo es un 1 y si recibo un valor negativo es un 0
      - Puede servir para clasificar un correo de spam o no spam
      - Hay un problema para calcular la derivada en 0
    - Sigmoide, salida entre 0 y 1 en clasificación binaria, es derivable
      - Se encuentra en capas finales
    - tanh(Tangente hiperbólica), Capa ocultas, represtar relaciones no lineales
      - Ej: Se usa dentro de las capas intermedias 
      - Son curvas no lineales, problema del desvanecimiento del tangente
      - Ayuda a que el modelo tenga más complejimiento
      - La salida es entre -1 y 1
    - ReLU, si recibo valores negativos los anulo con 0 y si recibo valores positivos devuelvo el mismo valor
- Perceptrón:
  - Es una nuerona que puede tener varias entradas y tiene como activación la función identidad
  - Es el modelo $w^Tx+b>=0$
  - Unidad más básica de una red neuronal
- Nuerona de regresión
  - $y = w^Tx+b$
  - Puede complejizar con muchas capas y conexiones entre neuronas
- ¿Cómo se hace el aprendizaje?
  - Vamos a tener un conjunto de datos(entradas y salidas), el modelo debe intentar hacer un prognóstico de esa salida(acercarse lo más posible a y)
  - Sabemos si se aproxima o no con una función de pérdida(que tan bien el modelo está haciendo la tarea)
    - Tenemos que minimizar la función de pérdida calculando la derivada o en vectores el vector gradiente
    - Dependiendo de la función, definimos la función de pérdida
      - Puede ser MSE(Promedio de errores al cuadrado/error cuadrático medio), entre otros.
    - Método del descenso de la gradiente:
      - La gradiente nos da la dirección de mayor crecimiento de la función, para saber el mínimo(menor crecimiento) su inverso nos dará la dirección de menor crecimiento
  - Con la grandiente que nos de una función de descenso actualiza los valores de w, b 
- Cuando hacemos el entrenamiento en función de nuestros recursos computacionales debemos definir:
  - **Época/epoch:** Un recorrido completo de los datos de entrenamiento
  - **Lote/batch:** Subconjutno de observaciones calculados para calcular la gradiente. Su tamaño B, se llama batch size
    - Para recorrer una época se divide en lotes/batches
  - **Actualización(Update o training step):** Un paso que modifica los pesos y el sesgo entrenables usando el gradiente de un lote y la tasa de aprendizaje


## Materiales de clase
- [Clase 12](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase12.pdf)
- [Resumen clase 12](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Resumenes/Resumen12.pdf)
- [Notebook revisado en clase](https://colab.research.google.com/github/andres-merino/AprendizajeAutomaticoInicial-05-N0105/blob/main/2-Notebooks/12-Perceptron-Lineal.ipynb)