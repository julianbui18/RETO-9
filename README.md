# RETO 9 - LISTAS
1. Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.

**SOLUCION**
```python
# Ingresar cantidad de datos
cantidad = int(input("Cantidad de valores a promediar "))
# Crear la lista para guardar los valores
valores = []
# Pedir los valores y guardarlos en la lista
for n in range(cantidad):
    numero = float(input("Ingrese el valor " + str(n + 1) + ": "))
    valores.append(numero)
# Calcular la suma de los valores
suma = 0
for numero in valores:
    suma += numero
# Calcular el promedio
if cantidad > 0:
    promedio = suma / cantidad
    print("El promedio es: " + str(promedio))
else:
    print("No hay valores para calcular el promedio.")
```

2. Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.
   
**SOLUCION**
```python
# Ingresar cantidad de elementos
cantidad = int(input("Ingrese la cantidad de elementos de los arreglos "))
# Crear las listas
arreglo1 = []
arreglo2 = []
# Pedir los elementos del primer arreglo
for n in range(cantidad):
    numero1 = float(input("Ingrese el valor " + str(n + 1) + " del primer arreglo: "))
    arreglo1.append(numero1)
# Pedir los elementos del segundo arreglo
for n in range(cantidad):
    numero2 = float(input("Ingrese el valor " + str(n + 1) + " del segundo arreglo: "))
    arreglo2.append(numero2)
# Calcular el producto punto
producto_punto = 0
for n in range(cantidad):
    producto_punto = producto_punto + (arreglo1[n] * arreglo2[n])
# Imprimir el resultado
print("El producto punto es: " + str(producto_punto))
```

3. Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.

**SOLUCION**
```python
# Ingresar el tamaño del arreglo
cantidad = int(input("Ingrese la cantidad de elementos de los arreglos "))
# Crear el arreglo
arreglo = []
# Llenar el arreglo
for n in range(cantidad):
    numero = int(input("Ingresar el número " + str(n + 1) + ": "))
    arreglo.append(numero)
# Crear un nuevo arreglo para los números distintos de cero
no_ceros = []
# Contar cuántos ceros hay
contador_ceros = 0
for n in range(cantidad):
    if arreglo[n] != 0:
        no_ceros.append(arreglo[n])
    else:
        contador_ceros = contador_ceros + 1
# Agregar los ceros al final
for n in range(contador_ceros):
    no_ceros.append(0)
# Mostrar el resultado
print("El arreglo con los ceros al final es: " + str(no_ceros))
```

4. Revisar que son los algoritmos de sorting, entender bubble-sort

Un algoritmo de sorting es un método para ordenar los elementos de un arreglo o lista según un criterio, como de menor a mayor o de mayor a menor. Estos algoritmos se usan para organizar datos de forma que sean más fáciles de buscar, analizar o presentar. Uno de los algoritmos más sencillos es el Bubble Sort (ordenamiento burbuja), que funciona comparando pares de elementos adyacentes e intercambiándolos si están en el orden incorrecto. Este proceso se repite varias veces hasta que todos los elementos están ordenados, haciendo que los valores grandes vayan "flotando" al final de la lista, como burbujas.

**JULIAN ESTEBAN BUITRAGO CRUZ**
