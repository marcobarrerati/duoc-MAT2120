[funciones](../README.md)
# Función cuadrática

Representa una parábola, su representación algebráica es la siguiente

```

f(x) = ax^2 + bx + c

Dónde a, b y c son números

f(x) = -x^2 -2x + 3

Dónde a = -1; b = 2; c = 3

"a" jamas puede ser 0

```
## Concavidad (a) a != 0
* Si el valor de "a" es menor a 0 será una función cóncava ; a<0 es negativo
* Si el valor de "a" es mayor a cero la curva estará hacia abajo; a>0 es positivo
## Punto de intersección

```

h(m)=3 m^(2)+4 m 
k(t)=-2 t^(2)+3+6

```

## Cálculos 
* Vertice
* Evaluar función con valor de entrada
* Evaluar posible valores de x1, x2 ingresando valor de salida
```python

import math

# Funciones cuadráticas
# Marco <marc.barrera@duocuc.cl>
# Referencia https://docs.google.com/spreadsheets/d/1pOdVzCqIB-64IU1r5daqA2VIrKRZB7JT/edit?usp=sharing&ouid=104977142821411523795&rtpof=true&sd=true
# 20211128

def ejeX(a, b):
    """
        Vertice X
        =SI(F5<>0;(H5*-1)/(2*F5);" ")
        Dónde F5 = a; H5 = b
    """
    x = 0
    if a < 0 or a > 0:
        x = (b*-1)/(2*a)  # Fórmula matemática
    return x


def ejeY(a, b, c, ejex):
    """
        Vertice Y
        =SI(F5<>0;(F5*B9*B9)+(H5*B9)+(J5);" ")
        Dónde F5 = a; B9 = ejeX; H5 = b; J5 = c
    """
    y = 0
    if a < 0 or a > 0:
        y = (a*ejex*ejex)+(b*ejex)+c  # Fórmula matemática
    return y


def evaluarVertice(a, b, c):
    """
        Cálcular X
    """
    x = ejeX(a, b)
    """
        Cálcular Y
    """
    y = ejeY(a, b, c, x)
    """
        Retornar valores
    """
    print("********")
    print("Vertice")
    print("X = ", x)
    print("Y = ", y)
    print("********")


def evaluarFuncionEn(b, c, valorDeEntrada):
    """
        Valor de entrada que deseas evaluar (x)
        =(F5*E8*E8)+(H5*E8)+J5
        Dónde F5 = a; H5 = b; J5 = c; E8 = valorDeEntrada
    """
    resultado = (a*valorDeEntrada*valorDeEntrada)+(b*valorDeEntrada)+c
    print("********")
    print("Evaluar en ", valorDeEntrada, ", resultado es ", resultado)
    print("********")


def evaluarValoresDeLaFuncion(a, b, c, valorDeSalida):
    """
        =SI.ERROR((($H$5*-1)+RAIZ(($H$5*$H$5)-4*$F$5*($J$5-E12)))/(2*$F$5);" ")
        =SI.ERROR((($H$5*-1)-RAIZ(($H$5*$H$5)-4*$F$5*($J$5-E12)))/(2*$F$5);" ")
        Dónde H5 = b; F5 = a; J5 = 3;
    """
    try:
        x1 = ((b*-1)+math.sqrt((b*b)-4*a*(c-valorDeSalida)))/(2*a)
        x2 = ((b*-1)-math.sqrt((b*b)-4*a*(c-valorDeSalida)))/(2*a)
        print("********")
        print("Para que la función tome el valor de ", valorDeSalida)
        print("Los posibles resultados son")
        print("X1 = ", x1)
        print("X2 = ", x2)
        print("********")
    except:
        print("No puedo calcular los posibles resultados par ala función, intenta con otros número 🤓")


# Usar funciones

a, b, c = 0.5, -4, 3

evaluarVertice(a, b, c)

evaluarFuncionEn(b, c, valorDeEntrada=20)

evaluarValoresDeLaFuncion(a, b, c, valorDeSalida=10)

```