# RETO 10 💀

## Ejercicio 1
- Desarrolle un programa que permita realizar la suma/resta de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.
```python
matriz_1 = [[9, 2, 1], 
            [5, 7, 0], 
            [8, 3, 4]]

matriz_2 = [[1, 1, 2], 
            [7, 8, 2], 
            [6, 8 ,9]]
matriz_suma = []
matriz_resta = []  

if len(matriz_1) == len(matriz_2) and len(matriz_1[0]) == len(matriz_2[0]):
    for fila in range(len(matriz_1)):
        fila_resultado_1 = []
        fila_resultado_2 = []
        
    for columna in range(len(matriz_1[0])):
        suma = matriz_1[fila][columna] + matriz_2[fila][columna]
        resta = matriz_1[fila][columna] - matriz_2[fila][columna]
        fila_resultado_1.append(suma)
        fila_resultado_2.append(resta)

        matriz_suma.append(fila_resultado_1) 
        matriz_resta.append(fila_resultado_2)
    print(f"Suma de matrices: {matriz_suma}")
    print(f"Resta de matrices: {matriz_resta}")

else:
    print("No se pueden sumar.")
```

## Ejercicio 2
- Desarrolle un programa que permita realizar el producto de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.
```python
matriz_1 = [[9, 2, 1], 
            [5, 7, 0], 
            [8, 3, 4]]

matriz_2 = [[1, 1, 2], 
            [7, 8, 2], 
            [6, 8, 9]]

if len(matriz_1[0]) == len(matriz_2):
    matriz_producto = []
    for fila in range(len(matriz_1)):
        fila_resultado = []

        for columna in range(len(matriz_2[0])):  
            suma_productos = 0

            for k in range(len(matriz_2)):  
                suma_productos += matriz_1[fila][k] * matriz_2[k][columna]

            fila_resultado.append(suma_productos)

        matriz_producto.append(fila_resultado)

    print("Producto de matrices:")
    for fila in matriz_producto:
        print(*fila)
else:
    print("No se pueden multiplicar.")

```

# Autor 🤖
- [Juan Carlos Polania Bolivar](https://github.com/Ciyuang)
