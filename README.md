# Tecnológico de Software  
## Materia: Fundamentos de Álgebra  
## Profesor: Jorge Javier Pedroza Romero
## Alumno: *Luis Edwuard Chay Ascorra*  
## Actividad #20
---
## Objetivo general 

El objetivo de esta actividad fue reforzar las operaciones matriciales fundamentales mediante su aplicación en Excel, representando imágenes como matrices y realizando con ellas transposición, suma, resta, multiplicación escalar y composición. Además, se busca practicar el uso de fórmulas, formato condicional y funciones matriciales en Excel, junto con la correcta documentación del proceso en Markdown dentro de un branch en GitHub, aplicando buenas prácticas de control de versiones y redacción técnica.

---
## Documentación de Matrices Originales (Imágenes 36×36) 

En esta sección documento como hice la construcción de cinco imágenes representadas como matrices de 36×36 en Excel. Cada imagen se generó utilizando una matriz numérica, donde cada número corresponde a un color específico del pixel art, la coloración visual no se realizó manualmente, sino mediante Formato Condicional basado en fórmulas, permitiendo convertir la matriz numérica en una imagen pixelada dentro de Excel. Este procedimiento facilita trabajar las imágenes como matrices para aplicar operaciones matemáticas posteriores. 

### 1. Matriz de Imagen Original 1 (36×36) 

#### Captura de la Hoja en Excel

<img width="720" height="746" alt="Captura de pantalla 2025-11-25 122828" src="https://github.com/user-attachments/assets/19b78347-7a7b-4c25-9ca4-d45b139f968a" /> 

#### Método Utilizado 

Se creó una matriz de 36 filas × 36 columnas, asignando un valor numérico para cada pixel (ej.: 1 = negro, 2 = azul oscuro, 3 = azul). 

Para “colorear” la imagen se aplicaron reglas de formato condicional: 

> Excel → Formato condicional → Nueva regla → “Usar una fórmula que determine las celdas para aplicar formato”

Para cada color se definió una fórmula del tipo:

```excel
=A1=1   → aplica color 1 → Negro
=A1=2   → aplica color 2 → Azul Oscuro 
=A1=3   → aplica color 3 → Azul 
=A1=4   → aplica color 4 → Gris Oscuro 
=A1=5   → aplica color 5 → Gris 
=A1=6   → aplica color 6 → Blanco
=A1=7   → aplica color 7 → Naranja
=A1=8   → aplica color 8 → Amarillo
```
Cada regla incluía un relleno de color distinto.
```excel
$A$1:$AJ$36
```
(un rango de 36 columnas de A a AJ). 

Fragmento de Ejemplo (solo 5×5 para demostración) 
| 1⬛ | 1⬛ | 2🟦 | 2🟦 | 2🟦 |
|---|---|---|---|---|
| 1⬛ | 2🟦 | 2🟦 | 8🟨 | 8🟨 |
| 2🟦 | 2🟦 | 8🟨 | 8🟨 | 8🟨 |
| 2🟦 | 8🟨 | 8🟨 | 8🟨 | 8🟨 |
| 8🟨 | 8🟨 | 8🟨 | 8🟨 | 8🟨 |

---
### 2. Matriz de Imagen Original 2 (36×36)

#### Captura de la Hoja en Excel

<img width="718" height="649" alt="Captura de pantalla 2025-11-25 164043" src="https://github.com/user-attachments/assets/aca514fc-ce3e-4424-83e5-f0ce6f6a2774" />

#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 1:

- matriz de 36×36

- valores numéricos para representar colores

- reglas de formato condicional basadas en fórmulas como:

```excel
=A1=1   → aplica color 1 → Negro
=A1=7   → aplica color 2 → Rojo 
=A1=8   → aplica color 3 → Amarillo 
=A1=12   → aplica color 4 → Naranja
=A1=14   → aplica color 5 → Verde 
=A1=6   → aplica color 6 → Blanco
```

Fragmento de Ejemplo (solo 5×5 para demostración) 

| 1⬛ | 7🟥 | 8🟨 | 12🟧 | 14🟩 |
|----|----|----|-----|-----|
| 1⬛ | 1⬛ | 7🟥 | 8🟨 | 6⬜ |
| 7🟥 | 8🟨 | 12🟧 | 14🟩 | 1⬛ |
| 8🟨 | 12🟧 | 14🟩 | 7🟥 | 6⬜ |
| 12🟧 | 14🟩 | 6⬜ | 1⬛ | 8🟨 |

---

### 3. Matriz de Imagen Original 3 (36×36)

#### Captura de la Hoja en Excel

<img width="621" height="636" alt="Captura de pantalla 2025-11-25 165552" src="https://github.com/user-attachments/assets/827e312e-4e36-4f9e-a86c-1527a64bd0c2" />

#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 1 y 2

#### Fragmento Ejemplo

| 9🩶 | 5⬛ | 1◼️ | 0⬜ | 9🩶 |
|----|----|----|----|----|
| 5⬛ | 9🩶 | 0⬜ | 1◼️ | 5⬛ |
| 1◼️ | 0⬜ | 5⬛ | 9🩶 | 1◼️ |
| 0⬜ | 5⬛ | 9🩶 | 1◼️ | 0⬜ |
| 9🩶 | 1◼️ | 0⬜ | 5⬛ | 9🩶 |

---

### 4. Matriz de Imagen Original 4 (36×36)

#### Captura de la Hoja en Excel

<img width="850" height="746" alt="Captura de pantalla 2025-11-25 172534" src="https://github.com/user-attachments/assets/0665a127-70cb-4954-a265-0fc516c94ac0" />

#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 1 , 2 y 3

#### Fragmento Ejemplo

| 0⬜ | 1⬛ | 1⬛ | 0⬜ | 8🟨 |
|----|----|----|----|----|
| 0⬜ | 0⬜ | 1⬛ | 0⬜ | 8🟨 |
| 0⬜ | 1⬛ | 0⬜ | 0⬜ | 8🟨 |
| 1⬛ | 0⬜ | 0⬜ | 1⬛ | 8🟨 |
| 8🟨 | 8🟨 | 7🟥 | 8🟨 | 8🟨 |

---

### 5. Matriz de Imagen Original 5 (36×36)

#### Captura de la Hoja en Excel

<img width="715" height="746" alt="image" src="https://github.com/user-attachments/assets/6e38b7d1-1f8f-41e5-9d0b-7706005be216" />

#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 1 , 2 , 3 y 4

#### Fragmento Ejemplo

| 11🟥 | 12🟥 | 11🟥 | 14🟨 | 0⬜ |
|-----|-----|-----|------|-----|
| 13🟧 | 13🟧 | 13🟧 | 11🟥 | 11🟥 |
| 13🟧 | 13🟧 | 13🟧 | 13🟧 | 11🟥 |
| 0⬜ | 14🟨 | 13🟧 | 13🟧 | 13🟧 |
| 11🟥 | 11🟥 | 0⬜ | 14🟨 | 11🟥 |

---

## Documentación de Matrices Traspuestas (Imágenes 36×36)

Tras construir las cinco matrices originales (36×36), se generó para cada una su matriz traspuesta.
La traspuesta de una matriz A consiste en intercambiar filas por columnas, es decir:

> El elemento en fila i, columna j pasa a la posición fila j, columna i.

Esto permite aplicar operaciones matriciales correctamente y visualizar cómo cambia la distribución del pixel art al reorganizar la matriz.

---

### 1. Traspuesta de la Imagen 1

Captura de la Hoja en Excel:

<img width="725" height="806" alt="image" src="https://github.com/user-attachments/assets/85887028-ea8c-44e9-a1c1-cfcbe18760f1" />

#### Método Utilizado:

En Excel, se utilizó la función:

```excel
=TRANSPONER(Lucario!A1:AK36)
```
### Importante:

Antes de escribir la fórmula, es necesario seleccionar un rango del mismo tamaño que la matriz original.
Como la matriz original es de 36 filas × 36 columnas, su traspuesta también será de 36×36.
En Excel moderno no necesitas presionar CTRL + SHIFT + ENTER, la fórmula matricial se confirma automáticamente.

--- 

### 2. Traspuesta de la Imagen 2

Captura de la Hoja en Excel:

<img width="707" height="687" alt="image" src="https://github.com/user-attachments/assets/ca096082-e0f2-4639-92ed-5c3b4a5295f6" />

#### Método Utilizado:

Se aplicó la misma fórmula adaptada al rango de la imagen 2:

```excel
=TRANSPONER(Charizar!A1:AK36)
```

---

### 3. Traspuesta de la Imagen 3

Captura de la Hoja en Excel:

<img width="603" height="690" alt="image" src="https://github.com/user-attachments/assets/9c112c8b-6df7-423c-b13d-335e94ec2015" />

#### Método Utilizado:

Fórmula usada:


```excel
=TRANSPONER(HollowKnight!A1:AK36)
```

---

### 4. Traspuesta de la Imagen 4

Captura de la Hoja en Excel:

<img width="857" height="803" alt="image" src="https://github.com/user-attachments/assets/e60ab6c0-a15a-415f-ad50-d1bc2fd30d06" />

#### Método Utilizado:

Fórmula usada:


```excel
=TRANSPONER(Snoopy!A1:AK36)
```

---

### 5. Traspuesta de la Imagen 5

Captura de la Hoja en Excel:

<img width="715" height="655" alt="image" src="https://github.com/user-attachments/assets/0756002c-7feb-46dc-b632-8c4b376e992f" />

#### Método Utilizado:

Fórmula usada:


```excel
=TRANSPONER(Foxy!A1:AK36)
```
