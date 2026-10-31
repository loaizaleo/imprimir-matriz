# imprimir-matriz

Programa en **C++** que pide por teclado los datos de una **matriz cuadrada** y la guarda en un archivo de texto.

## Objetivo

Practicar arreglos bidimensionales, lectura con `cin` y escritura de archivos con `fopen` / `fprintf`.

## Lenguaje

- **C++** (compilador `g++`)

## Archivos

| Archivo | Descripción |
|---|---|
| `printMatrix.cpp` | Pide el tamaño `M`, luego cada dato `[i][j]`, y escribe la matriz en `inputmatriz.txt`. |

## Uso

```bash
g++ printMatrix.cpp -o printMatrix
./printMatrix
```

Ejemplo con una matriz de 2 × 2:

```
Input size of matrix (mxm) : 2
data [1][1] : 1
data [1][2] : 2
data [2][1] : 3
data [2][2] : 4
```

Resultado en `inputmatriz.txt`:

```
1 2
3 4
```

## Notas

- Solo acepta números enteros.
- El arreglo se declara de 1000 × 1000 dentro de `main`, lo que ocupa unos 4 MB de la pila. En algunos sistemas (por ejemplo, Windows) esto puede hacer que el programa se cierre al iniciar. Se puede evitar declarando el arreglo como `static` o fuera de `main`.
