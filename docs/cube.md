
# Cp.Cube (Antes Table)


Crea una matriz indexada por uno o más índices permitiendo asignarle un valor a cada elemento de dicho índice.

La estructura de la función es la siguiente:

**result = cp.cube(axes, values=None, broadcast=True, dtype=None)**

**Axes:**  lista de axis de la matriz  
**Values (opcional):**  Lista de valores de la matriz. Puede ser una lista de cubos para crear un reporte.

**Ejemplos:**

1.  result = cp.cube([time])

1.  result = cp.cube([time,product])

1.  result = cp.cube([time,product],[10,20,30,40,50,60,70,80])

1.  result = cp.cube([time,product],cp.random)

**Ejemplo para crear un reporte:**

1.  result = cp.cube([index_reports],[report_1,report_2])
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk0MTQyNTgyNl19
-->