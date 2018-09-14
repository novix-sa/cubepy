# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. 
A labeled array is an array which dimensions or indexes are defined by a name.
This is an example of a 2 dimensional array called *"Sales"* indexed by *"product"* and *"region"*.

```python
Sales = cp.cube([product, region],[[  1,  2,  3], [ 11, 12, 13], [ 21, 22, 23]])
```
In this case the dimension *"product"* is defined as:
```python
product = cp.index('product',['Item 1', 'Item 2', 'Item 3'])
```
and the dimension *"region"* as:
```python
region = cp.index('region',['North','South','Center'])
```
so that the "Sales" cube can be visualized as:

![Sales](http://cubepy.org/files/sales.png)

The main goal of Cubepy is provide mathematical operations and functions for easy computing array calculations, leaving to the calculation engine the tasks of understanding array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
Lets suppose we have another cube called "Price" defined as follows:

```python
Price = cp.cube([product], [ 2, 3, 4])
```

![price](http://cubepy.org/files/price.png)

Then we can calculate *"Revenue"* as follows:

```python
Revenue = Sales * Price
```

![revenue](http://cubepy.org/files/revenue.png)

In this case the * operation between cubes is interpreted as follows:

For all dimensions that are common to each cube the * mathematical operation is applied element wise. For all dimensions that are not equal the engine broadcast the operation for the not equal index. The dimensions of the result is the union of dimensions of the operating variables. 

It is easier to interpret the operation with numbers:
![array product](http://cubepy.org/files/array%20product.png)

## Understanding Array Operations
### Escalar with array
### Equally dimensional arrays
### Operations with arrays of different dimensions
### Operations with arrays and indexes
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzMzc1OTgzNDIsLTg4NDc2ODY2NCw4Nz
IyNTI0MjAsLTE2Nzk4ODg2NTMsLTIxMzc2MTI2NTYsLTc5MzU5
NzgzNywxOTgxNjQ5NzY1LDE2NjI1ODIyOTEsLTE2MzY3Mjc3Mj
QsLTM2OTM4NzExMiwtMTA3NDYzNDU3NiwxMjU3NTY1OTI5LDE0
MjE2Njk4MjMsMTExOTYxMzczNywxNDMyMDM5NjQyLC0yMzIzND
YwMzYsMTg3Mjg2ODczMSwxNDY4NjYwNjc5LDY3MDc2NTI4Niwt
MTQwODY4Mzk2MV19
-->