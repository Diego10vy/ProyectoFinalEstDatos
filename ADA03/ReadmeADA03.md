# ADA 03 - Listas Dobles: Gestor de Catálogo de Películas

## Descripción de la Actividad
Esta ADA consistió en crear un sistema completo de gestión para un catálogo de películas, extrayendo los datos desde un archivo **Movies.csv**. La estructura de datos clave utilizada fue una **Lista Doblemente Ligada** implementada desde cero en **C**. Esto implicaba que cada nodo no solo apuntaba al siguiente, sino también al anterior. El programa permite la **carga inicial de datos** y ofrece un menú interactivo para realizar operaciones esenciales como:
* Búsqueda por ID.
* Inserción de nuevas películas.
* Eliminación de registros (con confirmación).
* Actualización de datos.

## Reflexión Personal
Esta fue una ADA dificil, ya que implementamos la **Lista Doblemente Ligada** desde cero, lo que significaba manejar **dos punteros** (`next` y `prev`) por cada nodo, duplicando el cuidado con la memoria dinámica el mayor reto no fue solo crear la lista, sino también dominar la lectura y el *parsing* del archivo **CSV**, que es un formato de datos del mundo real. Tuvimos que asegurarnos de que el programa pudiera buscar, insertar y borrar elementos en cualquier posición de la lista, manteniendo siempre la integridad de los enlaces tanto hacia adelante como hacia atrás, lo cual me hizo comprender cómo las listas enlazadas son más flexibles que los arreglos fijos.

## Contenido de la Carpeta

* **[Problema01](./Problema01)**: Contiene el código fuente `Peliculas_listas.c`, el archivo de datos `Movies.csv` y los archivos de documentación complementarios.