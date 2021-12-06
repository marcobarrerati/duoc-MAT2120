[Funciones](../README.md)
# Caso 2

La altura promedio f(x), en centímetros, de un niño durante su primer año de vida se puede determinar mediante la función f(x) = (2/3)x+48, donde x es el tiempo transcurrido, en meses, desde que nace

a) Defina la variale dependiente e independiente, indicando unidad de medida

✅ La variable dependiente corresponde a la altura promedio en centímetros

✅ La variable independiente corresponde al tiempo representado en meses

b) Escriba el dominio de la función y el dominio contextualizado.

✅ El dominio es el tiempo en meses

✅ El dominio contextualizado es el intervalo de meses, es decir [0,12]

c) Determine e interprete f(6) y f(8)
```python
# f(x) = (2/3)x+48
# f(6) = (2/3)*6+48 
print((2/3)*6+48) # 52.0
# f(8) = (2/3)*8+48
print((2/3)*8+48) # 53.333333333333336
```
d) Si un niño mide 50cm, ¿Cuántos meses de vida tiene?

```
f(x) = (2/3)x+48

50 = (2/3)*x+48
50 - 48 = (2/3)x
2 = (2/3)x
2 * 3 = 2x
6 = 2x
6 / 2  = x
3 = x
```

e) ¿Es posible calcular la edad de un niño si su estatura es de 68 cm?

```

f(x) = (2/3)x+48

68 = (2/3)x+48
68 - 48 = (2/3)x
20 = (2/3)x
20 * 3 = 2x
60 = 2x
60 / 2  = x
30 = x

```

## Análisis de caso

La regla de Young nos permite calcular la dosis en mg de medicamento que se debe administrar a niños desde 1 hasta 12 años de edad, conocida la dosis normal en adultos. Si la dosis normal para adulto es de 500mg entonces la regla de Young dice que la función

f(x) = 500x/x+12

Nos da la dosis para un niño, con x la edad del niño en años.

a) Defina la variable dependiente e independiente, indicando unidad de medida
```

✅ La variable dependiente es miligramos de medicamento

✅ La variable independiente es la edad del niño representada en años

```
b) Escriba el dominio de la función y dominio contextualizado
```

✅ El dominio matemático R{-12}

✅ Dominio contextualizado [1, 12] el rango de edad del niño

```
c) ¿Es correcto administrar 512 mg de paracetamol a un niño de 10.5 años?
```python

x = 10.5
m = (500*x)/(x+12)
print("para un niño de ", x, "años corresponde ", m, " mg de medicamento")

```

d) Determine e interprete f(7)
```python
# f(7) = (500*x)/(x+12)
x = 7
m = (500*x)/(x+12)
print("A un niño de  ", x, " años, se tiene que administrar ",
      m, " mg de medicamento")
```

e) ¿Cuánto medicamento se le debe administrar a un niño de 2 años y 6 meses?


```python
# 6 meses equivalen a 2.5 año o a 0.5 años. 2 años 6 meses = 2.5 años

x = 2.5
m = (500*x)/(x+12)
print("A un niño de  ", x, " años, se tiene que administrar ",
      m, " mg de medicamento")

```

f) Si a un niño se le administra 180mg de paracetamol, ¿cuál es su edad?
```

f(x) = (500*x)/(x+12)

180 = (500x)/(x+12)
180 (x+12) = 500x
(180x) + (180*12)
180x + 2160 = 500x
180x + 2160 = 500x 
2160 = 500x - 180x
2160 = 320x
2160/320 = x
6.75 = x

```
Crear función para calcular edad en base a miligramos de medicamento, buscando la inversa
```
f(x) = 500x/(x+12)
m = 500x/(x+12)
m(x+12) = 500x
mx+12m = 500x
12m = 500x-mx
12m/500-m = x
```
Evaluar con python, ingresando miligramos en la variable mg
```python
n=1
mg = 180
termino=500*1/(1+12)
while termino<mg:
    n=n+1
    termino=(500*n)/(n+12)
print(f'f({n})={termino}')
```