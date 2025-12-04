# ADA 07 - Implementación de Tablas Hash

## Descripción de la Actividad
El objetivo de esta ADA fue comprender y aplicar la estructura **Tabla Hash** como la estructura de datos más eficiente para búsquedas ($O(1)$ en promedio). Se desarrollaron dos aplicaciones en **C**, cada una ilustrando una técnica de control de colisiones:

1.  **Aplicación 01 (Estudiantes):** Uso de **Direccionamiento Abierto (Sondeo Lineal)**. La clave (matrícula) se mapea a una posición, y si está ocupada, se busca linealmente el siguiente espacio disponible.
2.  **Aplicación 02 (Tabla de Símbolos):** Uso de **Encadenamiento (Listas Ligadas)**. La clave (nombre del identificador *string*) se mapea a una "cubeta" de la tabla, y todas las colisiones se almacenan en una lista ligada adjunta a esa posición.

## Reflexión Personal
Esta ADA fue muy buena al introducir la idea de velocidad **casi instantánea** en operaciones de inserción y búsqueda, si se maneja bien la **función hash**. Entender los dos enfoques principales para las colisiones fue muy educativo. El **Sondeo Lineal** (AP01) es simple de implementar, pero sufre de la desventaja del *clustering primario*, haciendo las búsquedas lentas al tener que recorrer la tabla. En contraste, las **Listas Ligadas** (AP02) son más robustas y flexibles para diferentes tipos de claves (*strings*), siendo el diseño preferido para la **Tabla de Símbolos** donde la clave es una cadena de texto. La dificultad principal estuvo en implementar correctamente las funciones **hash para números** y, sobre todo, la **función hash para cadenas** (como la DJB2 o similar) y la gestión de la memoria dinámica en las listas de encadenamiento.

## Contenido de la Carpeta

* **[ADA07_AP01](./ADA07_AP01)**: Aplicación para el registro de estudiantes con manejo de colisiones por **Sondeo Lineal**.
* **[ADA07_AP02](./ADA07_AP02)**: Aplicación para la tabla de símbolos con manejo de colisiones por **Listas Ligadas (Encadenamiento)**.