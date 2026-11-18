¿Cuántas filas devuelve cada consulta y por qué son distintas? Explicá con ejemplos concretos de los datos qué filas se eliminaron con UNION.
La Consulta 1 devuelve 11 filas. La Consulta 2 devuelve 14 filas. Eso tiene que ver con que la función UNION elimina duplicados y UNION ALL no. Los productos 103,104 y 106 se repiten en ambas sucursales. 

¿Por qué UNION ALL es más eficiente que UNION? ¿Qué operación adicional realiza UNION internamente que consume más recursos?
UNION ALL es más eficiente porque unifica tablas pero no realiza la tarea de eliminar duplicados como sí ocurre con UNION.

¿En qué casos de negocio usarías cada uno? Dá al menos dos ejemplos reales distintos a los del ejercicio.
Usaría UNION si quiero ver qué productos tenemos en el sistema cargados y UNION ALL para ver cuáles productos tiene cada sucursal.

¿Qué pasa si las columnas de ambas consultas no coinciden en número o tipo? ¿Qué error genera SQL?
Msg 205: All queries combined using a UNION, INTERSECT or EXCEPT operator must have an equal number of expressions in their target lists.
