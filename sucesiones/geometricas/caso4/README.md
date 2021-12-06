[Matemática Aplicada MAT2120 - Sucesiones Geométricas](../README.md)
# Caso 4

Una casa se arrienda por 2 años, considerando que durante este periodo el arriendo se incrementará todos los meses en una cantidad constante. Si el quinto mes de arriendo se pagará $204.000 y el décimo tercer mes $252.000 ¿mal será el valor del arriendo del primer y último mes?

```
24 meses

Mes1	mes2	mes3	mes4	mes5	mes6	mes7	mes8	mes9	mes10	mes11	mes12	mes13
								204000															252000

204000 + 8d = 252000

8d = 252000 - 204000
8d = 48000
d=480000/8
d=6000

6000*4 = 24000

Mes 1 
204000-24000 = 180000

Mes 24
180000+144000 = 324000

```

```python

a1, d, suma = 190000, 3500, 0

for n in range(1,25):
    termino = a1 + (n-1)*d
    print(f"{termino}")
    suma = suma + termino

print(suma)

```