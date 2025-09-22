# Proyecto-TC1031
## Inventario de productos de una tienda

Este proyecto consiste en un sistema sencillo que administra el inventario de productos de una tienda.  
La idea es poder registrar productos con sus datos principales (sku, nombre, categoría, precio, stock y fecha de caducidad)  
y realizar operaciones de ordenamiento para apoyar decisiones como reabastecer, comparar precios o detectar productos próximos a caducar.

Ejemplo de funcionamiento:

 Producto: Leche entera 1L 
 
 Precio: 24.90 pesos  
 
 Stock: 12 piezas  
 
 Caducidad: 30/11/2025  

El sistema debe poder ordenar por precio, por stock y por fecha de caducidad.

De esta forma, puedo listar primero los productos con menor stock,

o ver cuáles están por vencer.


## SICT0302: Toma decisiones

### Selecciona un algoritmo de ordenamiento adecuado al problema y lo usa correctamente
Para este avance decidí usar Selection Sort y Merge Sort.

Uso Selection Sort porque es un algoritmo sencillo de implementar y me sirve como punto de partida para validar que los comparadores funcionan correctamente.  
Por otro lado, implemento también Merge Sort porque es más eficiente cuando se trabaja con listas grandes, ya que garantiza un rendimiento de O(n log n) incluso en el peor caso y además es estable, lo cual resulta útil cuando hay empates en atributos como precio o fecha de caducidad.  
De esta forma, puedo comparar ambos algoritmos y justificar su uso en diferentes situaciones.


## SICT0301: Evalúa los componentes

### Hace un análisis de complejidad correcto y completo para los algoritmos de ordenamiento usados en el programa

El algoritmo Selection Sort tiene complejidad O(n²) en el mejor, promedio y peor caso. El tiempo de ejecución crece de manera cuadrática conforme aumenta el número de productos en el inventario, por lo que solo resulta práctico para listas pequeñas.

Merge Sort tiene complejidad de O(n log n) en promedio y en el peor caso. Gracias a su estrategia de dividir y combinar, permite ordenar listas grandes de manera más eficiente y, al ser estable, conserva el orden relativo de los productos con el mismo valor en un campo.

Selection Sort me sirve como referencia didáctica y para pruebas iniciales, mientras que Merge Sort es la opción para manejar el inventario completo con un desempeño aceptable.


## SICT0303: Implementa acciones científicas

### Implementa mecanismos para consultar información de las estructuras correctos y útiles dentro de un programa


### Implementa mecanismos de lectura de archivos correctos y útiles dentro de un programa


### Implementa mecanismos de escritura de archivos correctos y útiles dentro de un programa
