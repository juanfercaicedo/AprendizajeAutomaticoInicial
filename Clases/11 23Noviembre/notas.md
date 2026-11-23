# Clase 10
## Aprendizaje Supervisado
  - **Overfitting:** Cuando el rendimiento en el entranamiento es mucho mejor que en las pruebas
      - El modelo memorizó los datos del entrenamiento
    - **Underfitting:** Si en el entranimiento no logra aprender, está subajustado, para resolverlo hay que seguirle entrenando
  - Un modelo debe generalizar sin hacer overfitting o underfitting
  - Un modelo mientras más complejo se hace, se va sobreajustado(Overfitting)
- Mientras probamos varios tipos de modelos, va a pasar lo siguiente
  - Si le damos más datos o más iteraciones con más variables, los modelos se van a hacer más complejos
  - Los datos se van a ajustar en función del tiempo
- La prueba siempre va a estar debajo del entrenamiento, la diferencia máxima es del 10%
## Algorítmo kNN
- A k no se le suele dar números pares para evitar los impares
- Lo ideal es que K sea igual a números primos
- Cuando gana un grupo porqué tiene más valores(elementos) dentro de un grupo.
  - Podemos utilizar **voto ponderado**, por ejemplo la distancia, en donde hacemos $n * 1/d$, donde n son la cantidad de elementos de un mismo grupo y de la distancia
  - También se conoce como **promedio ponderado**

## Materiales de clase
- [Clase 10](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Clases/Clase10.pdf)
- [Notebook revisado en clase](https://github.com/andres-merino/AprendizajeAutomaticoInicial-05-N0105/blob/main/2-Notebooks/10-kNN.ipynb)