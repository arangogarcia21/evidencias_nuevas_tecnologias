<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

# Promedio 
```Python:
notas_estudiantes = {
    'Juan': [3.2, 4.5, 5],
    'Maria': [4.2, 3.5, 4.3],
    'Pedro': [3.9, 2.5, 4.8]
}

def calcular_promedio(notas):
    if len(notas) == 0:
        return 0  
    suma = sum(notas)
    promedio = suma / len(notas)
    return promedio

for estudiante, notas in notas_estudiantes.items():
    promedio = calcular_promedio(notas)
    print(f'{estudiante}: El promedio es de = {promedio:.2f}')
```



