<!-- No borrar o modificar -->
[Inicio](./index.md)

# Sesión 2

## Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:
## While

<!-- Su documentación aquí -->

## Solicita al usuario que ingrese una lista de números y encuentra el número mayor y el menor.

## Punto 1:
```python:
numeros = []
cantidad = int(input("Ingrese la cantidad de números: "))

while cantidad > 0:
    numero = float(input("Ingrese un número: "))
    numeros.append(numero)
    cantidad -= 1

if numeros:
    maximo = numeros[0]
    minimo = numeros[0]

    for numero in numeros:
        if numero > maximo:
            maximo = numero
        if numero < minimo:
            minimo = numero

    print(f"El número mayor es {maximo} y el número menor es {minimo}")
else:
    print("No se ingresaron números.")

```

## Solicita al usuario un número e imprime la suma de los números pares entre 1 y ese número.

## Punto 2:
```python:
numero_limite = int(input("Ingrese un número: "))
suma = 0
numero_actual = 2

while numero_actual <= numero_limite:
    suma += numero_actual
    numero_actual += 2

print(f"La suma de los números pares hasta {numero_limite} es {suma}")

```

## Solicita al usuario una cadena e imprime cuántas vocales contiene.

## Punto 3:
```python:
cadena = input("Ingrese una cadena de texto: ")
cadena = cadena.lower() 

vocales = 'aeiou'
contador = 0

for letra in cadena:
    if letra in vocales:
        contador += 1

print(f"La cadena contiene {contador} vocales.")

```

## Solicita al usuario un número y muestra su tabla de potencias desde 1 hasta 10.

## Punto 4:
```python:

numero_base = int(input("Ingrese un número: "))
potencia = 1

while potencia <= 10:
    resultado = numero_base ** potencia
    print(f"{numero_base} ^ {potencia} = {resultado}")
    potencia += 1


```

## Solicita al usuario una lista de números y calcula la media aritmética.

## Punto 5:
```python:

numeros = []
cantidad = int(input("Ingrese la cantidad de números: "))

while cantidad > 0:
    numero = float(input("Ingrese un número: "))
    numeros.append(numero)
    cantidad -= 1

if numeros:
    suma = sum(numeros)
    media = suma / len(numeros)
    print(f"La media aritmética de los números ingresados es {media}")
else:
    print("No se ingresaron números.")

```

## Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:
## for

## Solicita al usuario una lista de números y calcula la suma de sus elementos.

## Punto 1:
```python:
numeros = input("Ingrese una lista de números separados por espacios: ").split()
suma = 0

for numero in numeros:
    suma += float(numero)

print(f"La suma de los números es: {suma}")

```

## Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:
## for

## Solicita al usuario una lista de números e imprime cuántos de ellos son pares.

## Punto 2:
```python:
numeros = input("Ingrese una lista de números separados por espacios: ").split()
cantidad_pares = 0

for numero in numeros:
    if int(numero) % 2 == 0:
        cantidad_pares += 1

print(f"La cantidad de números pares en la lista es: {cantidad_pares}")

```

## Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:
## for

## Solicita al usuario un número y muestra su tabla de multiplicar usando range().

## Punto 3:
```python:
numeros = input("Ingrese una lista de números separados por espacios: ").split()
cantidad_pares = 0

numero = int(input("Ingrese un número para mostrar su tabla de multiplicar: "))

for i in range(1, 11):
    producto = numero * i
    print(f"{numero} x {i} = {producto}")

```

## Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:
## for

## Solicita al usuario un número e imprime los números pares desde 2 hasta ese número.

## Punto 4:
```python:
numero_limite = int(input("Ingrese un número: "))

for i in range(2, numero_limite + 1, 2):
    print(i)


```

## Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:
## for

## Solicita al usuario un número y muestra la secuencia de números pares desde 2 hasta ese número.

## Punto 5:
```python:
numero_limite = int(input("Ingrese un número: "))

if numero_limite >= 2:
    for i in range(2, numero_limite + 1, 2):
        print(i)
else:
    print("El número debe ser mayor o igual a 2 para mostrar números pares.")

```