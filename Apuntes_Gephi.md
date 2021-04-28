# APUNTES DE GEPHI

## 1. Carga de archivos 
- Arrancamos y seleccionamos el proyecto a subir.
- Cuando se carga, notificaciones si hay un error.
- Tipo de grafo: mixto, dirigido, etc.
- Cuando existen varios grafos con varias aristas podemos elegir.


### 1.1 Vista general
- Mover la red, con el botón derecho del ratón.
- Izquierda: Apariencia (modificaciones de vista), Distribución de nodos.
- Derecha: Estadísticas para datos que me pueden ser intersantes. Correr algunas de estas optiones provoca que la herramienta habilite una serie de funcionalidades.
           Filtros 

### 1.2 Laboratorio de datos
- Características de cada nodos
- Botón derecho en la tabla de los nodos y click en "visualizar vista en grafo" me enseña el nodo dentro del grafo en vista general.

### 1.3 Previsualización
- Cuando ya he terminado todo, voy y lo miro

### 1.4 Otros
- Modularidad: busca relaciones entre nodos y los agrupa en comunidades.
- Esto supondrá una ampliación en las tablas de gephi.



## 2. Apariencia
- Extraer información que no esposible cuando se carga una red cambiando cómo se observan os grafos.
- T inferior: nombre de las etiquetas
    - En izquierda superior cambiar tamaño, color etc.

- Si no hay estadística, no vamos a poder trabajar con partición. Hay que calcular (por ejemplo, la modularidad).
- Distribución de ajuste de etiquetas para evitar superposición.
- Con el grado, se cambia el tao del nodo.


### 2.1 Información Particular sobre un nodo.
- Poándome sobre él con la flecha superior, me muestra las relaciones.
- Si selecciono la flecha inferior izq. y pulso sobre un nodo, me muestra las características. Pueden editarse.


## 3. Algoritmos de distribución
- Visualizar la red de diferentes formas y obtener información que no es tan visible.
    - Izquierda inferior.

### 3.1 Algoritmos "Puros"
- Force Atlas
- Force Atlas 2 (mejorado)
- Fruchteman Reingold, más uniforme (atracción por fuerzas eléctricas y gravitatorias).
- OpenOrd, muy rápido para distribuir en comunidades. Después de éste se suele utilizar force atlas (1 o 2).


### 3.2 Algoritmos "No Puros"
- Se trata de algoritmos como 
    - Contracción, 
    - Expansión
    - Distribución aleatoria (sin orden especificado y poco significativo)
    - No overlap (evita solapamientos).
    - Rotar, que va girando el grafo según el ángulo que le voy introduciendo en el parámetro cada vez que ejecuto el algoritmo. 



## 4. Filtros
- Los filtros nos permiten mostrar diferentes partes de una red en base a una serie de características.
-  Se acude a la sección de filtros a la derecha de la pantalla y se arrastra el que se desee usar a la parte inferior. Si se nos piden datos sobre un nodo, basta con acudir al mismo y pulsar click derecho y seleccionar "data laboratory".
- Dinámico: Ego, k-core (red en la que al menos todos los nodos tienen un número determinado de relaciones), rango de grado (muy interesante, permite discriminar sobre qué nodos cumplen un determinado rango de relaciones).

#### MUY IMPORTANTE 
- Cuando se genera una determinada red creada con un filtro, podemos exportarla a un nuevo workspace (espacio de trabajo) y trabajar solamente sobre ella.

- Operadores: aquellos que cumplan una determinada condición.
    - Los más relevantes: NOT (1), Intersección (varias).
- Partición: Modularity class. Me permite visualizar aquellas redes que me interesen en función de la clase a la que pertenecen.


## 5. 