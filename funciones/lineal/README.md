[Matemática Aplicada MAT2120 - Funciones](../README.md)
# Función Lineal
Representa una linea reacta en un gráfico y su forma algebraica se representa de la siguiente manera
```

f(x) = mx + n

```
m y n son número reales
|Letra Estándar|Nombre|Descripción|
|--|--|--|
| **m** |pendiente| Es el valor que siempre acompañará a la x o la letra que se este ocupando. El nombre de este elemento es **pendiente**. Puede ser ascendente o descendente. Tiene que ver con el grado de inclinación que puede ser negativa o positiva|
| **n** |coeficiente de posición| es el número solo, sin letra. El nombre que recibe es "**coeficiente de posición**" también pude denominarse "origne, "valor inicial", "punto de corte y". Representa el punto de corte en el eje Y|

* Cuando la pendiente es positiva la función es creciente
* Cuando la pendiente es negativa la función es decreciente
* Cuando la pendiente es nula o constante (no sube o no baja)

### Formula para evaluar un valor de entrada
```python
# f(x) = mx+n

x, m, n = 100, -9780, 997560

f = m*x+n
print(f)

```
### Formula para evaluar un valor de salida
```
resultado = 381420
n = 997560
m = -9780
x = (resultado-n)/m
print(x)
```
**Formula de pendiente (m)**
```

m = (y2-y1)/(x2-x1)

```
**Formula de coeficiente de posición (n)**
```
n = -mx1+y1

```