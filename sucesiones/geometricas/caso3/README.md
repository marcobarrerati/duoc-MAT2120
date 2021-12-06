[Matemática Aplicada MAT2120 - Sucesiones Geométricas](../README.md)
# Caso 3

La tasa de crecimiento de la población de una ciudad es del 2% anual, Si la población actual es de 600.000 habitantes, se pide.

A) Si an representa la población al cabo de n años, determine los tres primeros términos de esta sucesión.

```
an = a1 * r^(n-1)

Año 1 = 600000 * 1.02 = 612000
Año 2 = 600000 * 1.02 * 1.02 = 62424000
Año 3 = 600000 * 1.02 * 1.02 * 1.02 = 636724.8
```
B) Indicar qué tipo de sucesión modela la población de dicha ciudad. Justifique su respuesta
```
Sucesión aritmética, la cantidad de personas aumenta en base al 2%
```
C) Escribir la expresión algebraica del término de lugar an
```
an = 612000*1,02^(n-1)
```
D) Determinar cuántos habitantes aproximadamente tendrá dentro de quince años.

```
a(15) = 612000*1,02^(15-1)
```

```python
a1, r, n = 612000, 1.02, 15
termino = a1*r**(n-1)
print(f”a({n})={termino}”)
```
E) ¿Cuántos años aproximadamente deben transcurrir para que la población alcance los 1.351.320 habitantes?


```python
import math
termino, a1, r = 1351320, 612000, 1.02
n=(math.log((termino/a1),r))+1
print(n)
```

### Práctica

