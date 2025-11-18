# Documentación de Ejercicios - Luis Edwuard Chay Ascorra

## Información General
- **Materia:** Fundamentos de Álgebra  
- **Tema:** Documentación de ejercicios de matrices  
- **Fecha:** 18 de Noviembre del 2025  
- **Estudiante:** Luis Edwuard Chay Ascorra  
- **Grupo:** 1A

## Objetivo de la Documentación
Este documento contiene la explicación y el proceso detallado de los ejercicios de matrices trabajados en clase. La finalidad es mostrar el razonamiento paso a paso y practicar el uso de Git con branches y el formato Markdown para estructurar documentación técnica.

---

## Ejercicios Realizados


### Identificación de matrices


Matriz identidad, porque la diagonal está compuestos por solo unos y los elementos fuera de la diagonal son ceros.

$$ A=
\begin{pmatrix}
1 & 0\\
0 & 1\\
\end{pmatrix}
$$
---
MUESTRA

Calcula la suma de A y B

$$ A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
9 & 10 & 11 \\
12 & 13 & 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
1 + 9 & 2 + 10 & 3 + 11 \\
4 + 12 & 5 + 13 & 6 + 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
10 & 12 & 14 \\
16 & 18 & 20 \\
\end{pmatrix}
$$

---
# EJERCICIOS
...
### Ejercicio 1: Clasificar matrices
> identificar el tipo de cada matriz según su estructura.
Se debe observar la posición de los números dentro de la matriz para determinar si es identidad, diagonal, cuadrada o triangular.

## :)

$$
A=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix},
\quad
B=
\begin{pmatrix}
3&0&0\\
0&-2&0\\
0&0&5
\end{pmatrix},
\quad
C=
\begin{pmatrix}
2&1&4\\
1&3&5\\
4&5&6
\end{pmatrix},
\quad
D=
\begin{pmatrix}
1&2&3\\
0&4&5\\
0&0&6
\end{pmatrix}
$$

**Respuesta:**
- **A:** matriz de identidad, *por que todos sus elementos en la diagonal son 1 y fuera 0*
- **B:** matriz diagonal, *por que todos sus elementos fuera de la diagonal principal son 0*
- **C:** matriz cuadrada, *por que tienen el mismo número de filas que de columnas*
- **D:** matriz triangular superior, *por que todos sus elementos debajo de su diagonal principal son 0*

#### Procedimiento
1. **Analizar la diagonal principal:** Verificar si contiene únicamente unos, valores distintos o una estructura específica.  
2. **Revisar los valores fuera de la diagonal:** Comprobar si son todos ceros o si existen valores distintos.  
3. **Determinar la forma de la matriz:** Según filas, columnas y ubicación de valores.  
   - *Nota:* La clave es comparar el patrón de ceros y la estructura general.


---

### Ejercicio 2: Operaciones básicas
> El objetivo de este ejercicio es practicar las operaciones fundamentales con matrices.
Se pide realizar sumas, restas, multiplicaciones y la transpuesta, aplicando correctamente las reglas para cada tipo de operación.
### Dadas las matrices:
$$
A=
\begin{pmatrix}
2&-1\\
3&4
\end{pmatrix},
\quad
B=
\begin{pmatrix}
5&2\\
-1&3
\end{pmatrix}
$$
### Calcula:
- **a)** A+B  
- **b)** 2A-B  
- **c)** AB  
- **d)** BA  
- **e)** A^T

**Procedimiento:**

**A)  A+B**

$$ A + B =
\begin{pmatrix}
2 + 5 & -1 + 2\\
3 - 1 & 4 + 3 
\end{pmatrix}
\quad
R =
\begin{pmatrix}
7 & 1\\
2 & 7
\end{pmatrix}
$$

> Proceso/Procedimiento

Comprobar que ambas matrices sean del mismo tamaño (2×2).

Sumar elemento por elemento: A[i][j] + B[i][j].

Colocar cada resultado en la posición correspondiente.

Nota: Revisar signos negativos para evitar errores.

<!-- aquí termina mi ejercicio A de E2 -->
---

**B) 2A-B**

$$ 2A = 
\begin{pmatrix} 
2 (2) & 2 (-1) \\ 
2 (3) & 2 (4) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
4 & -2 \\
6 & 8
\end{pmatrix}
$$

$$ 2A - B =
\begin{pmatrix}
4 - 5 & -2 - 2\\
6 + 1 & 8 - 3 
\end{pmatrix}
\quad
R =
\begin{pmatrix}
-1 & -4\\
7 & 5
\end{pmatrix}
$$

> Proceso/Procedimiento

Multiplicar cada elemento de A por el escalar 2.

Restar elemento por elemento la matriz B.

Verificar signos positivos y negativos.

Nota: La multiplicación por escalar siempre se hace antes de la resta.

<!-- aquí termina mi ejercicio B de E2 -->
---

**C) AB**

$$ AB = 
\begin{pmatrix} 
2 (5) + (-1) (-1) & 2 (2) + (-1) (-3) \\ 
3 (5) + 4 (1) & 3 (2) + 4 (3) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
11 & 1 \\
11 & 18
\end{pmatrix}
$$

> Proceso/Procedimiento

Confirmar compatibilidad: A es 2×2 y B también; la multiplicación es posible.

Aplicar regla fila por columna:

Resultado[i][j] = Σ (fila de A × columna de B).

Repetir para cada posición.

Nota: La multiplicación de matrices NO es elemento a elemento.

<!-- aquí termina mi ejercicio C de E2 -->
---

**D) BA**

$$ BA = 
\begin{pmatrix} 
5 (2) + 2 (3) & 5 (-1) + 2 (4) \\ 
-1 (2) + 3 (3) & -1 (-1) + 3 (4) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
16 & 3 \\
7 & 13
\end{pmatrix}
$$

> Proceso/Procedimiento

Verificar que BA también sea posible: ambas matrices son 2×2.

Aplicar la fórmula fila × columna.

Comparar con AB: Los resultados son distintos.

Nota: Esto demuestra que la multiplicación de matrices no es conmutativa.

<!-- aquí termina mi ejercicio D de E2 -->
---

**E) Aᵀ**

$$ A^T =
\begin{pmatrix}
2 & -1 \\
3 & 4
\end{pmatrix}^T
R=
\begin{pmatrix}
2 & 3 \\
-1 & 4
\end{pmatrix}
$$

> Proceso/Procedimiento

Intercambiar filas por columnas.

Mantener los valores sin alterar signos.

Escribir la nueva matriz transpuesta.

Nota: Aᵀ no cambia valores, solo su posición.
<!-- aquí termina mi ejercicio E de E2 -->


---

### Ejercicio 3: Multiplicación en cadena
> Este ejercicio busca verificar la propiedad asociativa de la multiplicación de matrices, demostrando que el orden en que se agrupan las matrices no altera el resultado:
(AB)C=A(BC).
### Dadas las matrices:

$$ A=
\begin{pmatrix}
1&2\\
3&4
\end{pmatrix},
\quad
B=
\begin{pmatrix}
2&0\\
1&3
\end{pmatrix},
\quad
C=
\begin{pmatrix}
1&1\\
0&2
\end{pmatrix}
$$

### Procedimientos:
### Verifica que (AB)C = A(BC)
> *Primero multiplico A por B*

$$ AB = 
\begin{pmatrix} 
1 (2) + 2 (1) & 1 (0) + 2 (3) \\ 
3 (2) + 4 (1) & 3 (0) + 4 (3) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
4 & 16 \\
10 & 12
\end{pmatrix}
$$

> *Despues multiplico B por C*

$$ AB = 
\begin{pmatrix} 
2 (1) + 0 (0) & 2 (1) + 0 (2) \\ 
1 (1) + 3 (0) & 1 (1) + 3 (2) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
2 & 2 \\
1 & 7
\end{pmatrix}
$$

> *Ahora multiplico (AB) por C*

$$
AB=
\begin{pmatrix}
4&6\\
10&12
\end{pmatrix}\cdot
\quad
C=
\begin{pmatrix}
1&1\\
0&2
\end{pmatrix}
$$

$$ AB \cdot C= 
\begin{pmatrix} 
4 (1) + 6 (0) & 4 (1) + 6 (2) \\ 
10 (1) + 12 (0) & 10 (1) + 12 (2) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
4 & 16 \\
10 & 34 
\end{pmatrix}
$$

> *A continuación multiplico A por (BC)*

$$
A=
\begin{pmatrix}
1&2\\
3&4
\end{pmatrix}\cdot
\quad
BC=
\begin{pmatrix}
2&2\\
1&7
\end{pmatrix}
$$

$$ A \cdot BC= 
\begin{pmatrix} 
1 (2) + 2 (1) & 1 (2) + 2 (7) \\ 
3 (2) + 4 (1) & 3 (2) + 4 (7) 
\end{pmatrix}
\quad
R=
\begin{pmatrix}
4 & 16 \\
10 & 34 
\end{pmatrix}
$$

> *Para finalizar comparamos los resultados para corroborar que son iguales (AB)C = A(BC)*

$$
(AB)C=
\begin{pmatrix}
4&16\\
10&34
\end{pmatrix}=
\quad
A(BC)=
\begin{pmatrix}
4&16\\
10&34
\end{pmatrix}
$$

#### Procedimiento
1. **Multiplicar A por B:**  
   - Aplicando fila × columna.  
2. **Multiplicar B por C:**  
   - Revisar compatibilidad de dimensiones.  
3. **Calcular (AB)C:**  
   - Usar el resultado de AB y multiplicarlo por C.  
4. **Calcular A(BC):**  
   - Multiplicar A por el resultado BC.  
5. **Comparar resultados:**  
   - *Nota:* Si ambas matrices finales coinciden, se verifica la propiedad asociativa.
---

# Respuestas:

## Ejercicio 1

- **A:** matriz de identidad
- **B:** matriz diagonal
- **C:** matriz cuadrada
- **D:** matriz triangular superior

## Ejercicio 2

**A) A+B**

$$ A+B=
\begin{pmatrix}
7 & 1\\
2 & 7
\end{pmatrix}
$$

**B) 2A-B**

$$ 2A-B=
\begin{pmatrix}
-1 & -4\\
7 & 5
\end{pmatrix}
$$

**C) AB**

$$ AB=
\begin{pmatrix}
11 & 1\\
11 & 18
\end{pmatrix}
$$

**D) BA**

$$ BA=
\begin{pmatrix}
16 & 3\\
7 & 13
\end{pmatrix}
$$

**E) Aᵀ**

$$ Aᵀ=
\begin{pmatrix}
2 & 3\\
-1 & 4
\end{pmatrix}
$$

## Ejercicio 3

**Comparación Final**

$$
(AB)C=
\begin{pmatrix}
4&16\\
10&34
\end{pmatrix}=
\quad
A(BC)=
\begin{pmatrix}
4&16\\
10&34
\end{pmatrix}
$$

---
### Conclusión breve 

*Clasifiqué matrices (identidad, diagonal, triangular), realicé operaciones básicas (suma, resta, productos, transpuesta) y verifiqué la asociatividad de la multiplicación; todo documentado en Markdown con LaTeX para dejar el proceso claro y presentable.*

...