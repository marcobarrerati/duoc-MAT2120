[Funciones](../README.md)
# Caso 1

Roberto a ingresado a trabajar a una pesquera, donde le pagan un sueldo base de $230000 más $3500 por cada hora extra.

Si sabemos que en el més de Enero trabajo 12 horas extras, ne Febrero 7 horas extras y en Marzo 23 horas extras

¿ Es posible calcular el sueldo de Roberto en cada mes ?

* La variable dependiente corresponde al sueldo de Roberto
* La varianle independiente corresponde al número de horas extras trabajadas por Roberto
```
f(x) = m+yx -> dónde "m" es el sueldo base, "y" es el valor por hora extra y "x" es la cantidad de horas extras

f(x) = 230000+3500x

```
```python

sueldo, valorhoraextra, horasextras = 230000, 3500, [12, 7, 23]

for m in horasextras:
    funcion = sueldo+valorhoraextra*m
    print("sueldo al trabajar ", m, " horas extras : ", funcion)

```
Si Roberto gano 293000 ¿ cuántas horas extras trabajo ?
```

293000 = 230000 + 3500x
293000 - 230000 = 3500x
63000 = 3500x
63000 / 3500 = x
18 = x

Roberto trabajao 18 horas extras

```