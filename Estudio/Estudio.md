# Estudio exámen en línea 18 de noviembre
## Preguntas clase 6
- Si varias características de un conjunto de datos aportan información parecida, ¿qué ganaríamos y qué podríamos perder al resumirlas en menos dimensiones antes de analizar los datos?
  - Lo que ganamos al reducir la dimensionalidad de los datos es mayor eficiencia computacional, menos redundancia y ruido dentro del modelo y por último la capacidad de graficar y visualizar los datos. Por otro lado lo que perdemos es la interpretabilidad de los datos y el detalle de los datos residuales.
- Al reducir cuatro características a dos componentes con PCA, ¿qué información revisarías para decidir si la representación es suficiente?
  - Utilizamos la varianza explicada acumulada(`explain_variance_ratio_`)
  - Mide el porcentaje de variabilidad de la información
- ¿Qué diferencia hay entre conservar dos atributos originales y construir dos componentes principales?
  - La diferencia entre seleccionar y extraer atributos es que al seleccionar seleccionamos en función de su relevancia de el conjunto de datos. Mientras si los extraemos estamos creando atributos apartir de atributos ya existentes, lo cuál puede ayudar a conter información útil para entrenar al modelo.
-  Si conservas menos valores singulares al reconstruir una matriz, ¿qué esperas que ocurra con la información representada?
   - Al disminuir los valores singulares, mayor será la comprensión y la eliminaciuón del ruido, pero también será mayor la pérdida de fidelidad respecto a los datos originales.
 - En el ejemplo de preferencias, ¿qué representan U, Σ y $V^T$?
   - Representa la fórmula del SDV(Single Descomposition Value)
- ¿Qué precaución tomarías antes de aplicar e interpretar PCA sobre variables categóricas codificadas como números?
  - No podemos aplicar PCA sobre categorías numéricas, ya que esté mide las varianzas y las distancias euclideanas, asumiendo que los números representen magnitudes continuas y proporcionales
- ¿Cómo cambia la aproximación de una matriz de preferencias al conservar uno, dos o más valores singulares?
  - Mediante SVD, cada valor singular adicional incorpora una nueva dimensión de gusto, haciendo que la reconstrucción pase de mostrar una tendencia general uniforme a capturar preferencias cada vez más específicas y personalizadas.
## Preguntas clase 7
- Si el Profesor Oak pierde las etiquetas de «Tipo» y solo conserva estadísticas numéricas de los Pokémon, ¿qué similitudes podrían revelar los grupos obtenidos? ¿Por qué esos grupos no tendrían que coincidir con los tipos originales?
  - Los grupos obtenidos medirán la similitud entre las variables obtenidas
- ¿En qué se diferencia la pertenencia exclusiva de la pertenencia con superposición? ¿Puede un método jerárquico producir grupos exclusivos?
  - La permanencia exclusiva nos dice que un dato solo puede pertenecer a un grupo, es decir si pertenece a un grupo A no puede pertenecer a un dato B, mientras que la superposición nos dice que un dato puede pertenecer a más de un grupo, pero nos da un vector que contiene el grado de pertenencia de ese dato. Un grupo jerárquico si puede producir gurpos exclusivos, ya que divide los datos en diferentes ramas, es decir un dato solo puede pertenecer a una rama
- En el ejemplo del cuaderno, ¿qué asignaciones de k-means cambian, si las hay, al transformar los datos y cómo explicarías esas diferencias?
  - Las asignaciones cambian porque k-means agrupa midiendo la distancia euclidiana y es muy sensible a la escala de los datos. En los datos originales, la frontera es casi horizontal porque la segunda característica está multiplicada por 10 y domina por completo el cálculo de distancias; al aplicar StandardScaler o MinMaxScaler, ambas columnas pasan a escalas equivalentes y la frontera se inclina para capturar la separación real (produciendo grupos casi idénticos entre sí). Por el contrario, Normalizer escala cada observación por fila y proyecta los puntos sobre un círculo unitario, alterando por completo la geometría original y provocando que alrededor del 30 % de los datos cambien de grupo


## Materiales de estudio
- [Clase 06](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase06.pdf)
- [Resumen Clase 06](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Resumenes/Resumen06.pdf)
- [Clase 07](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase07.pdf)
- [Clase 08](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase08.pdf)
- [Resumen Clase 08](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Resumenes/Resumen08.pdf)