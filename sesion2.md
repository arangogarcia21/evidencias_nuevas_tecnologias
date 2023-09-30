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



