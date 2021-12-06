[Matemática Aplicada](../README.md)
# Matrices 
## ¿Qué es una matriz ?
Una matriz es un conjunto de elementos ordenados en filas y columnas
## ¿Qué nos indica el orden de la matriz?
Una matriz nos indica la cantidad de filas y columnas

### Sumar o Restar
***Condiciones*** El número de filas y columnas de las matrices tienen que ser iguales
```
1x2 + 1x2   # ✅
1x2 + 1x3   # 💔
```

### Multiplicar
***Condiciones*** El número de columnas de la primera matriz debe ser igual a número de filas de la segunda matriz “valores centro”

***Procedimientos*** Multiplicar números  de primera fila y primera matriz con los números de la primera columna de la segunda matriz, sumar sus resultados

|Función|Objetivo|Ejemplo de uso|
|--|--|--|
|dot|multiplicar 2 matrices|matrizA.dot(matrizB)|
```python
import numpy

A = np.array([[2,3,4],[5,6,8]])
B = np.array([[2,3,4],[5,6,8]])

N = A.dot(B) #here! ✅

```

|Función|Objetivo|Ejemplo de uso|
|--|--|--|
shape|Entrega la dimensión de la matriz|numpy.shape(matrizA)

```python
import numpy

numpy.shape(matrizA) #here! ✅
```

```python

import numpy

# Ejercicios 🏋️‍♀️

# una pequeña cadena tiene restaurantes de comida rápida em Santiago, Concepción y Antofagasta, en los que vende hamburguesa, completos y malteada. En un fin de semana, las cantidades de cada comida según cada sucursal se distribuyeron de acuerdo con la matriz 'v', donde las filas corresponden a los productos y las columnas a las sucursales, mientras que los precios, en pesos, de cada producto están expresados en la matriz 'p'.

# matriz p 1x3
p = numpy.array([[3600,900,1500]])

# matriz v 3x3
v = numpy.array([[1300,900,800],[2100,1700,1500],[1500,1200,900]])

# Dimensiones
print(numpy.shape(p))
print(numpy.shape(v))

# Multiplicación
print(p.dot(v))

# Dimensiones
print(numpy.shape(p.dot(v)))


# si i = p*v

# a - indicar el orden de las matrices p, v e i.
# p = 1x3
# v = 3x3
# i = 1x3

# b - determinar  la matriz i
# i = p.dot(v)

# c - interpretar los elementos v32, p12, i13
# v32 = 1200 malteadas en la sucursal de Concepción
# p12 = valor de los completos es $900
# i13 = la venta de productos en Antofagasta es de 5580000



# Multiplicar matriz de 2x2
a=numpy.array([[13,6],[21,32]])
print('a',a)
b=numpy.array([[4,6],[1,2]])
print('b',b)
d=a.dot(b)
print("d",d)
e=b.dot(a)
print("e",e)
f=a.dot(b)
print("f",f)


# Conmutación ... el orden de los factores si altera el producto
# Para multiplicar los numeros del centro deben ser iguales y la dimensión de la matriz resultado es equivalente a los números de los extremos (1x3 * 3x3)

```

