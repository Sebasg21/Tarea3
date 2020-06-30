# Universidad de Costa Rica

### Facultad de Ingeniería

### Escuela de Ingeniería Eléctrica

#### IE0405 - Modelos Probabilísticos de Señales y Sistemas

#### Sebastián Gómez Chaves; B42866
#### Grupo 02

# Tarea 3

1. A partir de los datos, encontrar la mejor curva de ajuste (modelo probabilístico) para las funciones de densidad marginales de X y Y.

Inicialmente con ayuda de la librería pandas se realiza la lectura de los datos brindados para poder manipularlos. Se definieron los vectores correspondientes para los ejes "x" y "y" con las dimensiones especificadas en los datos. Seguidamente se calcularon los vectores marginales respectivos, sumando los valores de probabilidades para cada columna y fila. Una vez obtenidos los vectores marginales para "x" y "y" se procedió a realizar una gráfica para cada caso para determinar la mejor curva de ajuste. 

![image.png](attachment:image.png)

![image.png](attachment:image.png)

Observando las gráficas se determina que la curva de mejor ajuste corresponde a la gaussiana, se define la función y se calculan los parametros de los vectores marginales. 
Al ingresar los parametros y su debido vector marginal en la función gaussiana definida anteriormente se obtienen las curvas de mejor ajuste para "x" y "y". Para visulizar de mejor manera que fuera una curva de ajuste adecuada de las densidades marginales se generaron gráficas.

![image.png](attachment:image.png)

![image.png](attachment:image.png)

2. Asumir independencia de X y Y. Analíticamente, ¿cuál es entonces la expresión de la función de densidad conjunta que modela los datos?

Para encontrar la expresión de la función de densidad conjunta que modela los datos, asumiendo la independecia de X y Y se determina al multiplicar las funciones de densidad marginales de X y Y encontradas anteriormente. De forma tal que si se observara en una gráfica 3D el plano XZ muestre la curva de densidad marginal de X y el plano YZ muestre la curva de densidad marginal de Y. 

3. Hallar los valores de correlación, covarianza y coeficiente de correlación (Pearson) para los datos y explicar su significado

Para encontrar los valores se trabaja con los datos "xyp.csv" pues se pueden extraer de maner más sencilla los vectores con todos los datos necesarios a "x", "y" y "p".

### Correlación: 
La correlación es el grado en el cual dos o más cantidades están linealmente asociadas. Para este caso se tomaron cada uno de los valores de los vectores y se multiplicaron para cada posicion en los vectores, esto es posible debido a que todos son de la misma longitud, y la suma de todas estas multiplicaciones brindan el valor de correlación. En otras palabras se realiza la suma de la multiplicación de todos los pares ordenados de "x" y "y" con su valor correspondiente de probabilidad. Arrojando un valor final de correlación de 149.54281000000012

### Covarianza:
Para determinar la covarianza se toma el valor de correlación y se le resta la multiplicación de valores medios de los modelos encontrados, al tratarse de una curva gaussiana, se sabe que el parametro "mu" corresponde al valor medio para cada modelo. Obeteniendo como resultado una covarianza de 0.18310502700205689

### Coeficiente de correlación (Pearson):
En cuanto al coeficiente de correlación, se determina tomando el valor de covarianza y dividiendolo entre la multiplicación de los parametros "sigma" de los modelos encontrados. Al realizar la operación se determinó un valor de 0.009207949908513998

4. Graficar las funciones de densidad marginales (2D), la función de densidad conjunta (3D)

Como se explicó en el primer segmento de la tarea, se habían determinado con anterioridad las gráficas de densidades marginales, se adjuntan a continuación nuevamente las mismas:

![image.png](attachment:image.png)

![image.png](attachment:image.png)

Para el caso de la función de densidad conjunta en 3D, se trabaja con los datos brindados, con cada par ordenado y la probabilidad respectiva de cada par. Se muestra a continuación la gráfica de la función.

![image.png](attachment:image.png)


```python

```
