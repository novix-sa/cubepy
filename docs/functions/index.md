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
eyJoaXN0b3J5IjpbMTE2NTczNDc5M119
-->