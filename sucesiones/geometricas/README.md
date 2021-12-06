[Matemática Aplicada MAT2120 - Sucesiones](../README.md)
# Sucesiones Geométricas

Una sucesión geométrica es una sucesión tal que entre un término y el anterior existe una razón constante. Dicho de otro modo, si dividimos dos términos consecutivos cualquiera el resultado es una razón r constante.

La sucesión

```
3, 6, 12, 24
```
Es geométrica porque
```
6/3 = 12/6 = 24/12  = 2
```
Por lo que la razón siempre es 2.

La sucesión 
```
4, 6, 9, 13.5, 20.25, …
```
Es geométrica porque
```
6/4 = 9/6 = 13.5/9 = 20.25/13.5 = … = 1.5
```
La sucesión geométrica es 
```
500, 400, 320, 256, 204.8, …
```
Pues la razón es 
```
400/500 = 320/400 = 256/320 = 204.8/256 = … = 0.8
```
Al igual que en las sucesiones aritméticas, la regularidad de las sucesiones geométricas nos permite encontrar una fórmula para el término general, Partiendo del primer término, a1, sabemos que el segundo se obtiene multiplicando el anterior por r
```
a2 = a1 * r
```
Y el tercero multiplicando el segundo por r
```
a3 = a2 * r = (a1 * r)r = a1 * r^2
```
Mientras que el cuarto es el anterior por r
```
a4 = a1 * r^2 * r = a1 * r^3
```
Si continuamos, podemos notar la recurrencia entre el subíndice, que marca la posición del término, con el exponente de la potencia. Finalmente, si tenemos el término de posición n, podemos obtenerlo como 
```
an = a1 * r^n-1
```

## Calculando términos de una sucesión geométrica

Podemos calcular los términos de una sucesión geométrica de dos maneras

1- Directamente con la fórmula del término de lugar n

Manual
```
an = a1r^n-1
```
Python
```python
a1	= 
r	=
n	=
termino=a1*r**(n-1)
print(f'a({n})={termino}')
```
2- Recursivamente, usando ciclos for desde i = 2 hasta i = n teniendo en cuenta que

Manual
```
ai = ai-1^r
```
Python
```python
termino =
r   =
for n in range(2,61): # empieza desde el 2
    termino=termino*r
print(f"a({n})= {termino}")
```

Determinando el lugar de un término en una sucesión geométrica

Tenemos dos manera de obtener el lugar que ocupa un término an cualquiera en este tipo de sucesión

1- Iterando con bucles while y en cada ciclo ir evaluando con la fórmula del término del lugar n.

2- Directamente usando logaritmos con la fórmula
```
n = logr(an/a1)+1
```
Calcular la razón dada dos posiciones
```python
pasos, derecha, izquierda = 3, 40, 5
r = (derecha/izquierda)**(1/pasos)
print(r)
```
Calcular la posición de un término de una sucesión geométrica conociendo el valor inicial y el valor de r 
```python
import math
termino, a1, r =413343, 7, 3
n= (math.log((termino/a1),r))+1
print(n)
```
## Análisis de caso

* [caso 1](caso1/README.md)
* [caso 2](caso2/README.md)
* [caso 3](caso3/README.md)
* [caso 4](caso4/README.md)