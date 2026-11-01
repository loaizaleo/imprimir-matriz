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
- Admite matrices de hasta 1000 × 1000. El arreglo se declara `static` para no llenar la pila (4 MB), lo que en Windows hacía que el programa se cerrara al iniciar.
