<p align="center">
  <img src="https://jorgebenitezlopez.com/tiddlywiki/pro/codefuente.jpg" alt="Código fuente" style="border:1px solid grey; max-width: 600px;">
</p>

Este documento es una introducción práctica y conceptual a la programación, desde los fundamentos hasta la arquitectura de software.

---

# 💡 Índice

- [1️⃣ ¿Qué es programar?](#1-qué-es-programar-)
- [2️⃣ ¿Cómo "hablamos" con una máquina?](#2-cómo-hablamos-con-una-máquina-)
- [3️⃣ Conocer el lenguaje para decirle lo que queremos](#3-conocer-el-lenguaje-para-decirle-lo-que-queremos-)
- [4️⃣ Estructuras de Datos y Algoritmos (A&ED)](#4-estructuras-de-datos-y-algoritmos-aed-)
- [5️⃣ Formas de uso / Buenas Prácticas](#5-formas-de-uso--buenas-prácticas-)

---

# 1️⃣ ¿QUÉ ES PROGRAMAR? 🤔

Los ordenadores no entiendían los lenguajes humanos como el español o italiano. Por eso, traducimos nuestros algoritmos a un lenguaje de programación, que sí pueden interpretar.

Estos lenguajes se ubican en una jerarquía que va desde el lenguaje máquina (binario) hasta los lenguajes de alto nivel como `Java`, `Python`, `JavaScript`, `C++`, entre otros.

---

# 2️⃣ ¿CÓMO "HABLAMOS" CON UNA MÁQUINA? 🖥️

Para comunicarnos con una computadora usamos una sintaxis específica. Aquí algunas formas comunes:

| Acción                | Ejemplo en JS         | Ejemplo en Python      |
|-----------------------|----------------------|-----------------------|
| Crear variable        | `let x = 2`          | `x = 2`               |
| Crear colección       | `[]`                 | `[]`                  |
| Comparar              | `==`, `>`            | `==`, `>`             |
| Definir función       | `function`           | `def`                 |
| Llamar función        | `miFuncion()`        | `mi_funcion()`        |
| Bucle                 | `for`, `while`       | `for`, `while`        |
| Condición             | `if`                 | `if`                  |
| Concatenar            | `+`                  | `+`                   |

> [!TIP]
> ¿Cuál es la forma correcta de definir una función en Python?
> - 🔵 `function miFuncion()`
> - 🔴 `def mi_funcion():`
> - 🟢 `let mi_funcion = function()`

---

# 3️⃣ CONOCER EL LENGUAJE PARA DECIRLE LO QUE QUEREMOS 🗣️

### 🔤 Alfabeto

- **Letras:** Caracteres como `A`, `z`.
- **Dígitos:** Números como `123`.
- **Símbolos:** Operadores y signos como `+`, `{}`, `[]`, `*`.
- **Espacios en blanco:** Separan palabras y símbolos.

### 🔠 Léxico (Lexis)

Conjunto de palabras válidas en el lenguaje. Ejemplo: `number` es válido, pero `if` es una palabra reservada y no puede usarse como nombre de variable.

### 📐 Sintaxis (Syntax)

Es la estructura correcta de las instrucciones. Por ejemplo, las funciones deben estar bien definidas y los condicionales correctamente escritos.

### 🧠 Semántica

La semántica se refiere al significado del código. Puede estar bien escrito, pero hacer algo diferente a lo esperado (por ejemplo, concatenar un string y un número puede dar un resultado inesperado).

**Otros conceptos importantes:**

- **Tipado o no tipado:** ¿El lenguaje obliga a definir tipos de datos? (ej. `Python`)
- **Compilado o Interpretado:** ¿el código se traduce antes o en tiempo de ejecución?

> [!TIP]
> ¿Cuál de las siguientes afirmaciones es correcta sobre el tipado en Python?
> - 🔵 Python permite mezclar tipos de datos sin restricciones (tipado débil).
> - 🔴 Python es fuertemente tipado: no permite mezclar tipos incompatibles sin conversión explícita.
> - 🟢 Python obliga a declarar el tipo de cada variable antes de usarla (tipado estático).

**Explicación:** Python es un lenguaje de tipado fuerte y dinámico. Esto significa que cada dato tiene un tipo y no puedes mezclar tipos incompatibles (por ejemplo, sumar un string y un número) sin conversión explícita. Sin embargo, no necesitas declarar el tipo de las variables: Python lo determina automáticamente en tiempo de ejecución.

> [!TIP]
> ¿Qué ocurre si usas una palabra reservada como nombre de variable?
> - 🔵 El programa funciona igual.
> - 🔴 El programa da error o se comporta de forma inesperada.
> - 🟢 El programa ignora la variable.

---

# 4️⃣ ESTRUCTURAS DE DATOS Y ALGORITMOS (A&ED) 🧱

Antes de construir una casa (nuestro programa), necesitamos conocer nuestros 
materiales y herramientas.

- **Estructuras de Datos:** Formas de organizar y almacenar datos.
    - Array (`[]`): Lista ordenada mutable
    - Objeto/Diccionario (`{}`): Pares clave-valor.
    - Tupla (`()`): Secuencia inmutable de elementos.
    - Otras: Lista enlazada, pila, cola, árbol, grafo...

> [!TIP]
> ¿Cuál es la principal diferencia entre una lista y una tupla en Python?
> - 🔵 Las listas son inmutables y las tuplas mutables.
> - 🔴 Las tuplas son inmutables y las listas mutables.
> - 🟢 No hay ninguna diferencia, son lo mismo.

- **Algoritmos:** Conjunto de instrucciones paso a paso, claras y finitas, diseñadas para realizar una tarea específica o resolver un problema. Son nuestras "herramientas", como una receta. Ejemplos:

    - **Búsqueda:** Encontrar un elemento en una estructura de datos (ej. búsqueda lineal vs binaria).
    - **Ordenamiento:** Organizar los elementos de una lista (ej. Quicksort, Merge Sort).
    - **Recorridos:** Visitar todos los nodos de un árbol o grafo.  
      👉 [Visualiza algoritmos aquí](https://algorithm-visualizer.org/)

```plaintext
Receta: Hacer un sándwich

1. Tomar dos rebanadas de pan.
2. Poner jamón y queso.
3. Tapar con la otra rebanada.
4. ¡Listo!
```
Así, un algoritmo es una serie de pasos claros y ordenados para resolver un 
problema y no es tan facil como parece: https://www.youtube.com/watch?
v=ajkglMnByFM

> [!TIP]
> ¿Cuál es la principal forma de medir la eficiencia o calidad de un algoritmo?
> - 🔵 Por la cantidad de líneas de código que tiene.
> - 🔴 Por la notación Big O, que indica cómo crece el tiempo o espacio requerido según el tamaño de los datos.
> - 🟢 Por el lenguaje de programación en el que está escrito.

**Explicación:** La notación Big O (O-grande) se usa para describir el comportamiento de un algoritmo cuando el tamaño de la entrada crece. Por ejemplo, un algoritmo de búsqueda lineal es O(n), mientras que uno de búsqueda binaria es O(log n). Esto ayuda a comparar la eficiencia de diferentes algoritmos, especialmente con grandes volúmenes de datos.

---

# 5️⃣ FORMAS DE USO Y BUENAS PRÁCTICAS EN GENERAL 🛠️

### ✅ Buenas prácticas

- **KISS:** Keep It Simple, Stupid (Hazlo simple): No reinventes la rueda, si lo haces complicado en unos días no lo entenderás ni tú ni tu equipo.
- **DRY:** Don't Repeat Yourself (Evita repetir código). La clave para saber que estás haciendo algo mal es si te repites.
- **Código limpio:** entendible, tabulado, nombres claros (`camelCase`), sin caracteres innecesarios.

> [!TIP]
> ¿Qué significa DRY en programación?
> - 🔵 Don't Repeat Yourself (Evita repetir código).
> - 🔴 Do Repeat Yourself (Repite el código).
> - 🟢 Dry Run Your code (Ejecuta tu código en seco).

### 🧭 Paradigmas de programación

Son estilos o enfoques para estructurar el código:

- **Imperativo:** Das instrucciones paso a paso.
- **Declarativo:** Dices qué quieres, no cómo hacerlo. Ej.: `array.map(...)` Algoritmos más optimizados que los que puedas escribir tú.
- **POO (Programación Orientada a Objetos):** Organiza el código en objetos que combinan datos y acciones.
- **Paradigma funcional:** Basado en funciones puras y evita el estado mutable.

> [!TIP]
> ¿Cuál es la diferencia entre el paradigma imperativo y el declarativo?
> - 🔵 El imperativo da instrucciones paso a paso, el declarativo dice qué se quiere lograr.
> - 🔴 El declarativo es más rápido siempre.
> - 🟢 No hay diferencia, son lo mismo.

### 🏗️ Patrones de diseño

Si los A&ED son las herramientas y materiales, los **Patrones de Diseño son los planos de la casa**. No te dicen cómo hacer un ladrillo, pero sí dónde poner un muro para que el software sea robusto, flexible y mantenible.

Son soluciones reutilizables a problemas comunes. Según el libro "Design Patterns" del "Gang of Four" (GoF), se agrupan en tres tipos: Creacionales, Estructurales y de Comportamiento.

| Patrón      | Descripción                                              | Ejemplo                  |
|------------|----------------------------------------------------------|--------------------------|
| Singleton  | Solo puede existir una instancia.                        | Una llave maestra        |
| Factory    | Crea objetos según lo que necesites.                     | Fábrica de autos         |
| Observer   | Notifica a varios componentes cuando algo cambia.        | Un timbre                |

> [!TIP]
> ¿Para qué sirve el patrón Singleton?
> - 🔵 Para asegurar que solo exista una instancia de una clase.
> - 🔴 Para crear muchas instancias diferentes.
> - 🟢 Para notificar a varios componentes.

### 🧱 Patrones de arquitectura

El plano general del sistema: cómo se organizan y comunican las partes.

- ¿Una sola planta (monolito) o varias (microservicios)?
- ¿Dónde va la cocina (backend) y el salón (frontend)?
- ¿Qué tan fácil es ampliar la casa (escalabilidad)?

Ejemplos: `MVC`, `Microservicios`, `Monolito`...

> [!TIP]
> ¿Qué es un patrón de arquitectura?
> - 🔵 Una forma de organizar y estructurar todo el sistema de software.
> - 🔴 Un tipo de variable.
> - 🟢 Un algoritmo de ordenamiento.

> [!TIP]
> ¿Qué patrón de arquitectura utiliza el framework Django?
> - 🔵 Microservicios
> - 🔴 Modelo-Vista-Controlador (MVC), aunque en Django se llama Modelo-Vista-Template (MVT)
> - 🟢 Event Sourcing

---
