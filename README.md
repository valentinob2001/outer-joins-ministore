# outer-joins-ministore
Practica M5 LEFT, RIGHT y OUTER JOIN

¿Por qué usaste LEFT JOIN para la Consulta 1 y no INNER JOIN? ¿Qué se perdería si usaras INNER JOIN?
Al utilizar INNER JOIN estaríamos descartando los casos sin concidencia, lo cual no es útil para encontrar los productos sin ventas asociadas.

¿Por qué usaste RIGHT JOIN para la Consulta 2? ¿Qué tabla está a la izquierda y cuál a la derecha en tu consulta?
En este caso, esta función sirve para mostrar todas las filas de la tabla derecha, sus concidencias con la izquierda y los casos en que no hay valores asignados, es decir, las filas son NULL. Mantuve el orden de la primera consulta, productos a la izquierda y ventas a la derecha

¿Qué representan los valores NULL en cada resultado? Explicá con un ejemplo concreto de los datos qué significa que venta_id sea NULL en la Consulta 1 y que producto_id de productos sea NULL en la Consulta 2.
Los valores NULL, en definitiva, son valores sin asignar a una celda. Yendo al ejemplo trabajado, cuando venta_id da NULL en la consulta 1 significa que el producto en cuestión no tiene ninguna venta asginada y cuando producto_id arroja el mismo valor en la consulta 2, siginifica que hay una venta registrada sin información de algún producto asociado

¿Cuándo usarías FULL OUTER JOIN en un caso real de negocio?
La mejor situación para aplicar tal herramienta se da cuando es necesario realizar un monitoreo y una supervisión general de ambas tablas, buscando valores nulos y patrones a simple vista para saber con los datos que se cuentan
