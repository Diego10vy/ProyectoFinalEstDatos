# ADA 01 - Pilas: Parser de Expresiones Aritméticas

## Descripción de la Actividad
Esta actividad consistió en desarrollar un programa en C++ capaz de interpretar y evaluar expresiones aritméticas complejas (con paréntesis y operadores de distinta prioridad como `^`, `*`, `/`, `+`, `-`).

El núcleo del proyecto se basó en dos algoritmos fundamentales:
1.  **Conversión Infija a Postfija:** Transformar expresiones estándar (ej. `3 + 4`) a Notación Polaca Inversa (ej. `3 4 +`) para eliminar la ambigüedad de los paréntesis.
2.  **Evaluación Postfija:** Calcular el resultado numérico procesando la cadena postfija.

Para lograr esto, se implementó una **Estructura de Datos tipo Pila (Stack)** de forma manual utilizando nodos enlazados y punteros, sin depender de la librería estándar de plantillas (STL) para la gestión de la pila.

## Reflexión Personal
Esta actividad me hizo comprender la utilidad práctica de las estructuras tipo Pila (LIFO) en el diseño de compiladores y calculadoras. YA que implementar la estructura manualmente mediante nodos enlazados y punteros, reforcé el manejo de memoria dinámica en C++, resolviendo desafíos lógicos relacionados con la gestión de direcciones de memoria, la jerarquía de precedencia de operadores matemáticos al igual que de tiempo.

## Contenido de la Carpeta

* **[Problema01](./Problema01)**: Contiene el código fuente `InfijoAPostfijoApp.cpp`, los archivos de prueba (`exp_infijas.txt`) y la documentación técnica de compilación.