# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Luis Edwuard Chay Ascorra
## Actividad \#16 - Matrices
## Fecha: Martes, 11 de Noviembre del 2025
---
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

A)  A+B

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

> *En este ejercicio sumé las dos matrices elemento por elemento, me aseguré de que tuvieran el mismo tamaño (2x2) y verifiqué los signos al sumar los valores negativos. El resultado fue una matriz con los valores correctos en cada posición.*

<!-- aquí termina mi ejercicio A de E2 -->

B) 2A-B

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

> *Primero multipliqué la matriz A por el escalar 2, luego realicé la resta con la matriz B, tuve cuidado con los signos negativos para no cometer errores en las operaciones. El resultado final fue una matriz 2x2 que muestra correctamente la resta entre ambas.*

<!-- aquí termina mi ejercicio B de E2 -->

C) AB

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

> *Aquí apliqué la multiplicación de matrices usando el método de filas por columnas, verifiqué que las dimensiones fueran compatibles y realicé cada producto con su respectiva suma. El resultado muestra cómo la multiplicación de matrices no se hace elemento a elemento, sino combinando filas y columnas.*

<!-- aquí termina mi ejercicio C de E2 -->

D) BA

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

> *Repetí la multiplicación, pero esta vez en el orden inverso (B por A), me di cuenta de que el resultado cambió por completo, lo que demuestra que la multiplicación de matrices no es conmutativa. También comprobé cada operación para confirmar que el resultado fuera correcto.*

<!-- aquí termina mi ejercicio D de E2 -->

E) Aᵀ

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

> *En este ejercicio calculé la transpuesta de la matriz A. Simplemente intercambié sus filas por columnas, manteniendo los valores en el mismo orden. El resultado confirma que la transpuesta cambia la orientación de la matriz, pero no sus valores.*

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