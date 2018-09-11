## cp.cube

Crea una matriz indexada por uno o más índices permitiendo asignarle un valor a cada elemento de dicho índice.

La estructura de la función es la siguiente:

```python
result = cp.cube(axes, values=None, broadcast=True, dtype=None)
```
**axes:**  lista de axis de la matriz  
**values (opcional):**  Lista de valores de la matriz. Puede ser una lista de cubos para crear un reporte.

**Ejemplos:**

```python
result = cp.cube([time])
result = cp.cube([time,product])
result = cp.cube([time,product],[10,20,30,40,50,60,70,80])
result = cp.cube([time,product],cp.random)
```

**Ejemplo para crear un reporte:**
```python
result = cp.cube([index_reports],[report_1,report_2])
```
 
<!--stackedit_data:
eyJoaXN0b3J5IjpbODcwNjU3MDBdfQ==
-->