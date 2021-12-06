[Matemática Aplicada MAT2120 - Sucesiones Geométricas](../README.md)
# Caso 1

Considere la sucesión geométrica: 4, 6, 9, … Determine

A) La razón geométrica
```
6/4 = 1.5
9/6 = 1.5
```
La razón geométrica es 1.5, es decir r = 1.5

B) La expresión del término de lugar n
```
an = a1 * r^(n-1)
an = 4 * 1.5^(n-1)
```
C) El término de lugar 60. Calcule con la forma directa y con la forma recursiva
```
an = a1 * r^(n-1)
```
Reemplazamos n
```
a60 = 4 * 1.5^(60-1)
```
Recursivo
```python
termino, r = 4, 1.5
for n in range(2,61): # empieza desde el 2
    termino=termino*r
print(f"a({n})= {termino}")
```
D) ¿Qué lugar ocupa en esta sucesión el término 68,34375? Use logaritmo

```
68,34375 = 4 * 1,5^(n-1)
68,34375/4 = 1,5^(n-1)
17,0859375 = 1,5^(n-1)

Log base 1,5 de 17,0859375 = n - 1

7 = n - 1
7 + 1 = n
n = 8
```

```python
import math
termino, a1, r = 68.34375, 4, 1.5
n=(math.log((termino/a1),r))+1
print(n)
````

En excel, Escribir primer termino en una celda y abajo multiplicar la celda anterior por la razón y copiar hacia abajo