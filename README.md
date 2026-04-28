# Sistema de Gestión de Empleados - Árbol Binario de Búsqueda (BST)

Este proyecto es una implementación en **C++** de un sistema de gestión de recursos humanos. Utiliza un **Árbol Binario de Búsqueda (BST)** para organizar a los empleados basándose en su código numérico, aplicando los principios de la **Programación Orientada a Objetos (POO)** en una arquitectura modular.

## Características Principales

El sistema permite realizar las siguientes operaciones a través de un menú interactivo en consola:

* **CRUD de Empleados:**
    * **Insertar** nuevos empleados (Código, Nombre, Cargo).
    * **Buscar** empleados rápidamente por su código.
    * **Actualizar** datos (Nombre y Cargo) de un empleado existente sin romper la estructura.
    * **Eliminar** empleados (el árbol se reorganiza automáticamente manejando casos de 0, 1 o 2 hijos).
* **Operaciones del Árbol (BST):**
    * Mostrar la raíz actual del árbol.
    * Recorridos de profundidad: **Inorden** (muestra empleados en orden ascendente), **Preorden** y **Postorden**.
    * Calcular la **altura** total del árbol.
    * Identificar y mostrar los **nodos hoja** (empleados sin subalternos directos en la estructura del árbol).

## Estructura del Proyecto

El código está dividido de forma modular siguiendo las mejores prácticas de C++ para separar la interfaz de la implementación:

* `Empleado.h` / `Empleado.cpp`: Declaración e implementación de la clase `Empleado` (datos estrictamente encapsulados).
* `ArbolBST.h` / `ArbolBST.cpp`: Declaración e implementación de la clase `ArbolBST` y su estructura interna y privada de `Nodo`.
* `main.cpp`: Punto de entrada del programa y gestión de la interfaz de usuario (menú).
* `.gitignore`: Archivo de configuración para evitar subir binarios compilados al repositorio.

## Tecnologías Utilizadas

* **Lenguaje:** C++ (Estándar C++11 o superior).
* **Paradigma:** Programación Orientada a Objetos (POO).
* **Estructura de Datos:** Árbol Binario de Búsqueda (BST).

## Cómo compilar y ejecutar localmente

### Requisitos previos
* Tener instalado un compilador de C++ (como GCC/MinGW).
* Una terminal, consola de comandos o VS Code.

### Pasos
1.  Clona o descarga este repositorio en tu computadora.
2.  Abre una terminal en la carpeta raíz del proyecto.
3.  **Compila** todos los archivos fuente juntos con el siguiente comando:
    ```bash
    g++ main.cpp Empleado.cpp ArbolBST.cpp -o SistemaRRHH
    ```
4.  **Ejecuta** el programa compilado:
    * En **Windows**:
        ```bash
        .\SistemaRRHH.exe
        ```
    * En **Linux/Mac**:
        ```bash
        ./SistemaRRHH
        ```

---
*Tarea Árboles / implementación personal para la demostración de estructuras de datos y árboles BST en C++.*
