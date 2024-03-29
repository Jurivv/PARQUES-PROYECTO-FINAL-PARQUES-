# Reto_7
1.Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
```python
i = 1  
while i <= 100:  
    print(i, i ** 2)  
    i += 1  
```

2.Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
```python
print("Números impares:")
i = 1
while i <= 999:
    print(i)
    i += 2 #se la suma 2 porque empieza en 3 los impares
```
```python
print("Números impares:")
i = 2
while i <= 1000:
    print(i)
    i += 1 #se la suma 1 porque empieza en 2 los impares
```
3.Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado
```python
n=int(input("Digite numero desde el cual descenderan los numeros primos siempre y cuando sea mayor o igual que 2"))  
i = n
while i >= 2:
    i -= 1
    if i % 2 == 0:
        print(i)
```

4.En 2022 el país A tendrá una población de 25 millones de habitantes y el país B de 18.9 millones. Las tasas de crecimiento anual de la población serán de 2% y 3% respectivamente. Desarrollar un algoritmo para informar en que año la población del país B superará a la de A.
```python
B = 18900000  
A = 25000000
tasa_A = 0.02  # 2%
tasa_B = 0.03  # 3%
año=int(input("ingrese un año"))
while B <= A:
    A *= (1 + tasa_A)
    B *= (1 + tasa_B)
    año += 1

print("La población del país B superará a la del país A en el año:", año)
```

5.Imprimir el factorial de un número natural n dado.
```python

```

6.Implementar un algoritmo que permita adivinar un número dado de 1 a 100, preguntando en cada caso si el número es mayor, menor o igual.
```python

```

7.implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.
```python
i = int(input("Digite un número entre 2 y 50: "))

if i < 2 or i > 50:
    print("El número digitado es inválido")
else:
    print(f"Divisores de {i}:")
    for n in range(1, i + 1):
        if i % n == 0:
            print(n)
```
8.Implementar el algoritmo que muestre los números primos del 1 al 100. Nota: use funciones
```python

def es_primo(i):
    if i < 2:
        return False
    for n in range(2, int(i**0.5) + 1):
        if i % n == 0:
            return False
    return True

i = 1
while i <= 100:
    if es_primo(i):
        print(i)
    i += 1
```
