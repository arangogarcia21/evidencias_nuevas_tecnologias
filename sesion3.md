<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 

## practicar con listas, tuplas, conjuntos y diccionarios en Python.

<!-- Su documentación aquí -->

# Listas

### Crear una lista que contenga los números del 1 al 10.
### Crear una lista que contenga los números del 1 al 10.
### Ordenar la lista en orden ascendente.
### Ordenar la lista en orden descendente.
### Encontrar el número más pequeño en la lista.
### Encontrar el número más grande en la lista.
### Contar el número de veces que aparece el número 5 en la lista.
### Elimina el número 5 de la lista.
### Agrega el número 11 a la lista.

```python:

numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

print("Lista original:", numeros)

numeros.sort()
print("Lista ordenada en orden ascendente:", numeros)

numeros.sort(reverse=True)
print("Lista ordenada en orden descendente:", numeros)

numero_minimo = min(numeros)
print("Número más pequeño:", numero_minimo)

numero_maximo = max(numeros)
print("Número más grande:", numero_maximo)

conteo_cinco = numeros.count(5)
print("Número de veces que aparece el 5:", conteo_cinco)

numeros.remove(5)
print("Lista después de eliminar el 5:", numeros)

numeros.append(11)
print("Lista después de agregar el 11:", numeros)
```

# Conjuntos

### Crear un conjunto que contenga los números del 1 al 10.
### Imprimir el conjunto.
### Agregar el número 11 al conjunto.
### Eliminar el número 5 del conjunto.
### Contar el número de elementos en el conjunto.
### Comprobar si el número 5 está en el conjunto.
### Comprobar si el número 11 está en el conjunto.

```python:

conjunto_numeros = set(range(1, 11))


print("Conjunto de números:", conjunto_numeros)


conjunto_numeros.add(11)


conjunto_numeros.remove(5)


num_elementos = len(conjunto_numeros)


esta_5 = 5 in conjunto_numeros


esta_11 = 11 in conjunto_numeros

print("Conjunto después de las operaciones:")
print("Elementos:", conjunto_numeros)
print("Número de elementos:", num_elementos)
print("¿5 está en el conjunto?", esta_5)
print("¿11 está en el conjunto?", esta_11)
```

# Tuplas

### Crear una tupla que contenga las palabras "Hola", "mundo" y "Python".
### Imprimir la tupla en el orden en que fue creada.
### Encontrar la primera palabra en la tupla.
### Encontrar la última palabra en la tupla.
### Contar el número de palabras en la tupla.
### No puedes eliminar elementos de una tupla ni agregar nuevos elementos. Sin embargo, puedes crear una nueva tupla con los elementos que deseas.
### Imprimir la nueva tupla.


```python:

mi_tupla = ("Hola", "mundo", "Python")

print("Tupla original:", mi_tupla)

primera_palabra = mi_tupla[0]
print("Primera palabra:", primera_palabra)

ultima_palabra = mi_tupla[-1]
print("Última palabra:", ultima_palabra)

numero_palabras = len(mi_tupla)
print("Número de palabras en la tupla:", numero_palabras)

nueva_tupla = (mi_tupla[0], mi_tupla[2], "Hola")

print("Tupla después de eliminar 'mundo' y agregar 'Hola':", nueva_tupla)
```

# Diccionarios

### Crear un diccionario de días de la semana.
### Imprimir el diccionario.
### Obtener el número del día de la semana "Lunes".
### Obtener el día de la semana correspondiente al número 2.
### Eliminar el día de la semana "Lunes" del diccionario.
### Imprimir el diccionario actualizado.

```python:

dias_semana = {
    "Lunes": 1,
    "Martes": 2,
    "Miércoles": 3,
    "Jueves": 4,
    "Viernes": 5,
    "Sábado": 6,
    "Domingo": 7
}


print("Diccionario de días de la semana:", dias_semana)


numero_lunes = dias_semana["Lunes"]
print("Número de 'Lunes':", numero_lunes)


dia_numero_2 = None
for dia, numero in dias_semana.items():
    if numero == 2:
        dia_numero_2 = dia
        break

print("Día correspondiente al número 2:", dia_numero_2)


del dias_semana["Lunes"]


print("Diccionario después de eliminar 'Lunes':", dias_semana)
```




