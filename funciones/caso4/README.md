[Funciones](../README.md)
# Caso 4

Los alumnos de recursos naturales modelaron la población de abejas en la ciudad de Santiago con la función lineal **A(t) = -9780t + 997560** donde t es el tiempo transcurrido en meses iniciada la investigación.

a) Defina las variables dependiente e independiente, indicadno unidad de medida

✅ La variable dependiente es el número de abejas

✅ La vairable independiente es el tiempo en meses

b) ¿Cuántas abejas había al inicio del estudio?

✅ El estudio comenzo con 997560 abejas

c) ¿En cuánto disminuye la cantidad de abejas mensualmente?

✅ La cantidad de abejas disminuye 9780 mensualmente

d) Los alumnos concluyen que las abejas desaparecerán al transcurrir 100 meses ¿Qué opinas de esa conclusión? Argumenta matemáticamente.

```
f(x)=mx+n   (m es pendiente y n es coeficiente de posición)

A(100) = -9780t + 997560
a los 100 meses aún quedan 19560 abejas

```
```python
# python

x, m, n = 100, -9780, 997560

f = m*x+n
print(f)  # 19560

```

c) Al momento de terminar el estudio había 381420 abejas. ¿Cuánto duró la investigación?
```
f(x)=mx+n

381420 = -9780t + 997560
381420-997560 = -9780t
-616140 = -9780t
-616140/-9780 = t
63 = t
```

```python
resultado = 381420
n = 997560
m = -9780
x = (resultado-n)/m
print(x)

```