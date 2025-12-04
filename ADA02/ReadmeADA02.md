# ADA 02 - Colas: Simulador de Atención al Cliente

## Descripción de la Actividad
El objetivo de esta actividad fue montar un **simulador de banco** con 3 cajas (o ventanillas). El programa, hecho en **C**, se encargó de modelar cómo llegan los clientes, se forman en la cola más corta y son atendidos. Todo el meollo del asunto era usar bien la estructura **Cola (Queue)**, que implementamos desde cero con **nodos y punteros**, siguiendo la regla **FIFO (el que llega primero, sale primero)**. Al final, el simulador arroja estadísticas para ver qué tan eficientes fueron las cajas y cuánto tiempo promedio esperó la gente.

## Reflexión Personal
Esta ADA estuvo bien para entender el **FIFO** y ver su aplicación real, lo más complejo fue hacer que toda la simulación funcionara a la vez, o sea, que el programa supiera cuándo llegaba un cliente nuevo (de forma aleatoria), cómo decidir a qué cola mandarlo (siempre a la menos saturada) y atender a la gente en las tres cajas al mismo tiempo. Poner bien los **punteros** de `frente` y `final` de las colas fue la parte más delicada, para que no se nos perdiera ningún cliente en la memoria.

## Contenido de la Carpeta

* **[Problema01](./Problema01)**: Contiene el código fuente `banco_simulador.c` y los archivos de documentación complementarios.