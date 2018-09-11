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
 
 
## cp.index

Crea un objeto index utilizando la lista de valores.
La estructura de la función es la siguiente:

```python
result = cp.index(values)
```

**Ejemplos:**

```python
result = cp.index(["Item 1","Item 2","Item 3"])
result = cp.index([2016,2017,2018])
result = cp.index(["item " + str(i+1)  for i in  range(100)])
```

Crear un indice a partir de filtrar elementos de una tabla que cumplen una condición:
```python
result = cp.index(cp.subset(input_data[input_data_cols=='Server']=='dedicated'))
```

En este caso la tabla es input_data, la columna con los datos es ‘Server’ y el valor ‘dedicated’.  
El resultado es el listado de clientes cuyo Servidor es Dedicado.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ4MjY3MTA5OSwxOTE3ODI2NDk5XX0=
-->