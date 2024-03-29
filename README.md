# Reto_7
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
