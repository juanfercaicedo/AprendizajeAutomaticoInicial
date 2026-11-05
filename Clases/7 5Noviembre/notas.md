# Clase 6
- Recall solo se puede hacer en binario
- 1 vs 1 (comparar 0 y 1) - hacemos una matriz 2x2
- 1 vs todos
---
## Agrupamientos o clúster
- Tratamos de medir numéricamente la cohesión
- Para medir la separación tenemos que comparar entre grupos uno a uno
- Hay que buscar maneras cuantitativas de medir la cohesión y la separación
    - Para medir la cohesión, calculamos el diámetro, medimos la separación entre los puntos extremos del grupo
    - Para medir la separación, es ver los puntos más cercanos entre grupos(separación entre dos grupos)
        - La separación se mide entre dos grupos midiendo que puntos son los más cercanos
- **Centroide del cluster**:
    -  Es el punto medio del clúster, calculado como el promedio de todos los puntos en el clúster
    - $\mu_i = \frac{1}{|C_i|} \sum_{x \in C_i} x$
- **Diámetro del clúster**:
    - Mide la distancia máxima entre dos puntos dentro del mismo clúster
    - $\text{diam}(C_i) = \max_{x, y \in C_i} d(x, y)$
- **Inercia**: 
    - Mide la cohesión interna de los clústeres, definida como la suma de las distancias cuadráticas entre cada punto y el centroide de su clúster
    - $I_i = \sum_{x \in C_i} d(x, \mu_i)^2$
    - Es mejor que el diámetro, cada clúster va a tener su propia inercia
- **Distancia promedio dentro del clúster**:
    - Mide la distancia promedio entre los puntos y el centroide del clúster
    - $S_i = \frac{1}{|C_i|} \sum_{x \in C_i} d(x, \mu_i)$
- **Cohesión de silueta**: 
    - Cada punto va a tener una cohesión de siluta, no va a ser del clúster
    - Mide la distancia promedio entre un punto y todos los demás puntos en el mismo clúster, para $x ∈ C$
    - $a(x) = \frac{1}{|C_i| - 1} \sum_{y \in C_i} d(x, y)$
- Ahora para **separación:**
- **Distancia entre clústeres:**
    - Mide la distancia mínima entre puntos de dos clústeres diferentes
    - $d(C_i, C_j) = \min_{x \in C_i, y \in C_j} d(x, y)$
- **Distancia entre centroides:**
    - Mide la distancia entre los centroides de dos clústeres
    - $d_c(C_i, C_j) = d(\mu_i, \mu_j)$
- **Separación de Silueta:**
    - Mide la distancia promedio entre un punto y todos los puntos en el clúster más cercano al que no pertenece, para x ∈ Ci
    - $b(x) = \min_{j \neq i} \frac{1}{|C_j|} \sum_{y \in C_j} d(x, y)$




---
## Materiales de clase
- [Resumen 05](https://andres-merino.github.io/AprendizajeAutomaticoInicial-05-N0105/2-Resumenes/Resumen05.pdf) - Agrupamientos del clúster