# Índice

- [1. ¿Qué es programar?](#1-qué-es-programar)
- [2. ¿Cómo "hablamos" con una máquina?](#2-cómo-hablamos-con-una-máquina)
- [3. Conocer el lenguaje para decirle lo que queremos](#3-conocer-el-lenguaje-para-decirle-lo-que-queremos)
- [4. Estructuras de Datos y Algoritmos (A&ED)](#4-estructuras-de-datos-y-algoritmos-aed)
- [5. Formas de uso / Buenas Prácticas](#5-formas-de-uso--buenas-prácticas)
  - [Buenas prácticas](#-buenas-prácticas)
  - [Paradigmas de programación](#-paradigmas-de-programación)
  - [Patrones de diseño](#-patrones-de-diseño)
  - [Patrones de arquitectura](#-patrones-de-arquitectura)

---

Este documento es una introducción práctica y conceptual a la programación, desde los fundamentos hasta la arquitectura de software.

# 1. ¿QUÉ ES PROGRAMAR?

Los ordenadores no entienden los lenguajes humanos como el español o italiano. Por eso, traducimos nuestros algoritmos a un lenguaje de programación, que sí pueden interpretar.

Estos lenguajes se ubican en una jerarquía que va desde el lenguaje máquina (binario) hasta los lenguajes de alto nivel como `Java`, `Python`, `JavaScript`, `C++`, entre otros.

# 2. ¿CÓMO "HABLAMOS" CON UNA MÁQUINA?

Para comunicarnos con una computadora usamos una sintaxis específica. Aquí algunas formas comunes:

*   ¿Cómo creo características? → `JS: let o const x = 2`, `En Python x:2` 
*   ¿Cómo creo una colección de cosas? → `Pythony JS: []`,
*   ¿Cómo hago una comparación? → `==`, `>`, etc.
*   ¿Cómo defino una acción? → `JS: function, Python: def`
*   ¿Cómo llamo una acción? → `nombreDeLaFuncion()`
*   ¿Cómo creo un bucle? → `for`, `while`, `map`, etc.
*   ¿Cómo creo una condición? → `if`
*   ¿Cómo concateno o uno cosas? → `+`
*   ¿Cómo controlo el flujo? → `callbacks`, `condicionales`, `funciones`

# 3. CONOCER EL LENGUAJE PARA DECIRLE LO QUE QUEREMOS

### 🔤 Alfabeto

*   **Letras:** Caracteres como `A`, `z`.
*   **Dígitos:** Números como `123`.
*   **Símbolos:** Operadores y signos como `+`, `{}`, `[]`, `*`.
*   **Espacios en blanco:** Separan palabras y símbolos.

### 🔠 Léxico (Lexis)

Conjunto de palabras válidas en el lenguaje. Ejemplo: `number` es válido, pero `if` es una palabra reservada y no puede usarse como nombre de variable.

### 📐 Sintaxis (Syntax)

Es la estructura correcta de las instrucciones. Por ejemplo, las funciones deben estar bien definidas y los condicionales correctamente escritos.

### 🧠 Semántica

La semántica se refiere al significado del código. Puede estar bien escrito, pero hacer algo diferente a lo esperado (por ejemplo, concatenar un string y un número puede dar un resultado inesperado).

**Otros conceptos importantes:**

*   **Tipado:** ¿el lenguaje obliga a definir tipos de datos? (ej. `TypeScript` vs `JavaScript`)
*   **Compilado o Interpretado:** ¿el código se traduce antes o en tiempo de ejecución?

# 4. ESTRUCTURAS DE DATOS Y ALGORITMOS (A&ED)

Antes de construir una casa (nuestro programa), necesitamos conocer nuestros materiales y herramientas.

*   **Estructuras de Datos**: Son formas especializadas de organizar y almacenar datos para poder acceder a ellos y modificarlos de manera eficiente. Son nuestros "materiales".
    *   **Array (`[]`)**: Una lista o colección ordenada de elementos.
    *   **Objeto/Diccionario (`{}`)**: Una colección de pares clave-valor.
    *   **Lista Enlazada, Pila, Cola, Árbol, Grafo...**: Estructuras más complejas para problemas específicos.

*   **Algoritmos**: Son un conjunto de instrucciones paso a paso, claras y finitas, diseñadas para realizar una tarea específica o resolver un problema. Son nuestras "herramientas". Es como una receta, pueden ser más eficientes que otras. Más información buscar: "Complejidad logarítmica, notación Big O". Ejemplos:
    *   **Búsqueda**: Encontrar un elemento en una estructura de datos (ej. Búsqueda lineal vs búsqueda Binaria).
    *   **Ordenamiento**: Organizar los elementos de una lista (ej. Quicksort, Merge Sort).
    *   **Recorridos**: Visitar todos los nodos de un árbol o grafo. Ejemplos. https://algorithm-visualizer.org/

**Ejemplo de algoritmo como receta (pseudocódigo):**

```plaintext
Receta: Hacer un sándwich

1. Tomar dos rebanadas de pan.
2. Poner una rebanada de jamón sobre una de las rebanadas de pan.
3. Poner una rebanada de queso sobre el jamón.
4. Tapar con la otra rebanada de pan.
5. ¡Listo! El sándwich está hecho.
```

Así, un algoritmo es una serie de pasos claros y ordenados para resolver un problema y no es tan facil como parece: https://www.youtube.com/watch?v=ajkglMnByFM

Dominar A&ED es fundamental para escribir código eficiente y optimizado.

# 5. FORMAS DE USO Y BUENAS PRÁCTICAS EN GENERAL

### ✅ Buenas prácticas:

*   **KISS**: Keep It Simple, Stupid (Hazlo simple): No reinventes la rueda, si lo haces complicado en unos días no lo entenderás ni tú ni tu equipo.
*   **DRY**: Don't Repeat Yourself (Evita repetir código). La clave pra saber que estás haciendo algo mal
*   **Código limpio**: entendible, tabulado, nombres claros (`camelCase`), sin caracteres innecesarios.

### 🧭 Paradigmas de programación

Son estilos o enfoques para estructurar el código:

*   **Imperativo**: Das instrucciones paso a paso.
*   **Declarativo**: Dices qué quieres, no cómo hacerlo. Ej.: `array.map(...)` Algoritmos más optimizados que los que puedas escribir tú.
*   **POO (Programación Orientada a Objetos)...**
*   **Paradigma funcional...**

### 🏗️ Patrones de diseño...

Si los A&ED son las herramientas y materiales, los **Patrones de Diseño son los planos de la casa**. No te dicen cómo hacer un ladrillo, pero sí dónde poner un muro para que el software sea robusto, flexible y mantenible.

Son soluciones reutilizables a problemas comunes. Según el libro "Design Patterns" del "Gang of Four" (GoF), se agrupan en tres tipos: Creacionales, Estructurales y de Comportamiento.

*   **Singleton**: Solo puede existir una instancia. Ej.: una llave maestra.
*   **Factory**: Crea objetos según lo que necesites.
*   **Observer**: Notifica a varios componentes cuando algo cambia. Ej.: un timbre.

### 🧱 Patrones de arquitectura...

El plano general del sistema: cómo se organizan y comunican las partes.

*   ¿Una sola planta (monolito) o varias (microservicios)?
*   ¿Dónde va la cocina (backend) y el salón (frontend)?
*   ¿Qué tan fácil es ampliar la casa (escalabilidad)?

Ejemplos: `MVC`, `Microservicios`, `Monolito`... 