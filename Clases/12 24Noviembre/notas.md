# Clase 11
## SVM(Support Vector Machine)
- Una aplicación lineal/función lineal/ mapa lineal
    - Las aplicaciones lineales son una función que permite que f(x + y) = f(x) + f(y)
    - Kernel de una aplicación son todos los valores en donde se hace 0
- Tres grupos puden ser linealmente separables si hay hiperplanos que los separen
- Cuando dos grupos son linealmente separables, hay infinitas rectas que las separan
  - Tenemos que determinar la mejor recta que los separa
  - Lo hacemos maximizando o minimizando la distancia entre los vectores de soporte
    - Vectores de soporte, los que están más pegados a la línea
- **Proyección ortogonal de un vector sobre otro vector**
- **Margen** la proyección de un vector sobre el otro
- Las máquinas de soporte vectorial estas enfocadas en hacer clasificación binaria cuando los grupos son linealmente separables. Plantea encontrar un plano de tal forma que todos los puntos queden de un lado y los otros puntos de otro, además generando un margen lo más grande posible
  - Encontrar el hiperplano que separe mejor a esos grupos
  - Mejor hiperplano, el que tenga el margen más grande
  - Margen, distancia de la recta hacia los vectores de soporte
  - Hacemos una proyección y nos genera un problema con una restricción(verdes en un lado y rojos a otro lado por ejemplo)
  - Para resolver el problema de optimización se utiliza multiplicadores de lagrange
  - Derivamos y se hace un sistema de ecuaciones
- Se puede suavizar el método para que cuando no son linealmente separables para que permita buscar un plano
  - Va a ignorar los puntos que no lo hacen linealmente separable y va a tratar de encontrar el plano que mejor se ajuste
- Cuando no podemos aplicar SVM podemos hacer una transformación de nuestro datos, es decir pasamos de dos dimensiones a tres
  - $(x1, x2) ->(x1, x2, x1^2 + x2^2)$
  - Por lo general nosotros debemos idear la transformación
  - También se le conoce como el truco del kernel   

## Materiales usados en clase
- [Clase 11](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase11.pdf)
- [Resumen Clase 11](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Resumenes/Resumen11.pdf)
- [Notebook revisado en clase](https://github.com/andres-merino/AprendizajeAutomaticoInicial-05-N0105/blob/main/2-Notebooks/11-SVM.ipynb)
  - Revisar documentación SVM sklearn para entender todos los parámetros