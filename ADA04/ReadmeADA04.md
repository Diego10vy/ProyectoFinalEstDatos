# ADA 04 - Árboles Binarios: Gestor de Estudiantes

## Descripción de la Actividad
El objetivo central de esta ADA fue desarrollar un sistema de gestión académica usando la estructura **Árbol Binario de Búsqueda (ABB)**, programado en **C**. La matrícula del estudiante se usa como clave para ordenar la información, lo que garantiza que las búsquedas e inserciones sean eficientes (logarítmicas). El sistema incluye:

* **Implementación Completa del ABB:** Desde la creación de nodos hasta las inserciones y la compleja función de eliminación.
* **Gestión de Datos Dinámicos:** Los estudiantes almacenan un número dinámico de calificaciones.
* **Reportes Clave:** Generación de listados ordenados por matrícula o promedio, y filtros para estudiantes con promedios por debajo o por encima de 70.
* **Operaciones Esenciales:** Inserción, eliminación y actualización de calificaciones.
* **Visualización:** Función para mostrar el árbol en formato ASCII.

## Reflexión Personal
Los **Árboles** fueron interesantes. Esta ADA fue clave para entender cómo los datos dejan de ser lineales y se vuelven jerárquicos. El desafío más grande, de lejos, fue la función de **eliminación de nodos** en el ABB, especialmente cuando el nodo a eliminar tiene dos hijos, que requiere buscar al sucesor in-order. Además, manejar las **calificaciones como arreglos dinámicos** dentro de cada `struct` de estudiante me obligó a ser super cuidadoso con la memoria (`malloc`/`free`) para evitar *memory leaks*. Al final,se logro un sistema que puede hacer búsquedas rapidísimas, algo que no se logra tan fácil con Listas o Colas.

## Contenido de la Carpeta

* **[Problema01](./Problema01)**: Contiene el código fuente `ABB.c` y los archivos de documentación complementarios.