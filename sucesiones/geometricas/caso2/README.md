[Matemática Aplicada MAT2120 - Sucesiones Geométricas](../README.md)
# Caso 2

El tercer término de una sucesión geométrica es 5 y el sexto término es 40.

Determine

A) La razón geométrica. Analice cuántos pasos hay entre ambos términos que se indica
```
3°	4°	5°	6°
5			40

5*r*r*r = 40
5*r^3 = 40
r^3 = 40/5
r^3 = 8
r = 3√8 = 2
```
La razón geométrica es 2

B) El primer término
```
La razón es 2
3/2 = 2.5
2.5/2 = 1.15

1°		2°	3°
1.25		2.5	5
```
C) La expresión del término de lugar n
```
an = 1.25*2^(n-1)
```
D) El octavo término. Calcule con la forma que estime conveniente.
```
an = 1.25*2^(8-1) = 160


160 = 1.25*2^(8-1)
```
E) ¿Qué lugar ocupa en esta sucesión el término 20480, Use logaritmo
```python

import math
termino, a1, r = 20480, 1.25, 2
n = (math.log((termino/a1),r))+1
print(n)

```
