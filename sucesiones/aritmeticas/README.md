[Matemática Aplicada MAT2120 - Sucesiones](../README.md)
# Sucesiones Aritméticas

Una sucesión aritmética es una sucesión tal que entre un término y el anterior existe una diferencia constante. Dicho de otro modo entre dos términos consecutivos cualquiera hay una distancia d fija

La regularidad de las sucesiones aritméticas permite encontrar una fórmula para el término general. Sabemos que el primer término es a1. El segundo término, entonces, tiene que ser

```
a2 = a1 + d
```

El tercer término es el segundo más la distancia, pero podemos escribirlo en términos del primer término

```
a3 = a2 + d = (a1 + d) + d = a1 + 2d
```

Y podemos hacer algo similar con el cuarto término

```
a4 = a3 + d = (a1 + 2d) + d = a1 + 3d
```

Podemos notar la recurrencia entre los subíndices y el coeficiente de d y escribir el término genérico como 

```
an = a1 + (n - 1)d
```

## Sucesiones monótonas

Una sucesión monótono creciente es una sucesión donde cada término es mayor o igual al anterior, es decir

```
an <= an + 1
```

Una sucesión monótona decreciente es una sucesión donde cada término es menor o igual al anterior, es decir

```
an >= an + 1
```


## Calcular término de una sucesión aritmética


Podemos calcular los términos de una sucesión aritmética de dos maneras

1- Directamente, usando la fórmula para el término de lugar n
```
an = a1 + (n + 1)d
```
2- Usando ciclos for desde i = 2 hasta i = n teniendo en cuenta que
```
ai = a1 - 1 + d
```


```python
# Por término 
a1, d, n	= 3, 6, 1
termino = a1+(n-1)*d
print(termino)


# Recursivo
termino	=
d	=
for n in range(1, 101):
	termino = termino + d
print(termino)

# Buscar posición de un término
termino	=
a1	=
d	=
n = ((termino-a1)/d)+1
print(n)
```

___

## Práctica

En una colonia de abejas, en el primer día de investigación, alumnos de ingeniería agrícola contabilizaron 3 abejas, el segundo día contabilizaron 9 y el tercero 15.
Si la cantidad de abejas se fue incrementando de manera constante, se pide

A) Indicar qué tipo de sucesión modela la cantidad de abejas. Justificar la respuesta.
```
Sucesión monótona creciente, porque sus valores van aumentando con una constante de 6 
```
B) Escribir la expresión del término de lugar n
```python
an = 3+(n-1)*6
```
C) Determinar cuántas abejas había el vigésimo día
```python
a1, d, n  = 3, 6, 20
termino = a1+(n-1)*d
print(termino) # 117 abejas
```
D) Determinar cuantas abejas había a los 30 días
```python
a1, d, n  = 3, 6, 30
termino = a1+(n-1)*d
print(termino) # 177 abejas
```
E) ¿Cuántos días deben transcurrir para que se puedan contabilizar 333 abejas?

```
333 = 3 + (n-1)*6
333 - 3 = (n-1)*6
330 / 6 = n-1
55 = n-1
55 + 1 = n
56 = n
```

```python
termino, a1, d = 333, 3, 6
n = ((termino-a1)/d)+1
print(n) # 56 días
```