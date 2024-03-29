# Reto_7
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
