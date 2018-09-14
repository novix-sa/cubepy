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
Lets suppose we have another cube called:

```python
Price = cp.cube([product], [ 2, 3, 4])
```

![price](http://cubepy.org/files/price.png)

Then we can calculate *"Revenue"* as follows:

```python
Revenue = Sales * Price
```

![revenue](http://cubepy.org/files/revenue.png)

In this case the * operations between cubes is interpreted as follows:
For all dimensions that are common to each cube the * mathematical operation is applied element wise. For all dimensions that are not equal the engine broadcast the operation for the not equal index. The dimensions of the result is the union of dimensions of the operating variables. 
It is easier to interpret the operation with numbers:
(insert graph to explain operation)
![enter image description here](https://drive.google.com/file/d/17D-2mvTpjc4hnDPj1_M_q6OSFHzaIm4r/view?usp=sharing)
## Understanding Array Operations
### Escalar with array
### Equally dimensional arrays
### Operations with arrays of different dimensions
### Operations with arrays and indexes
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTk2ODg2OTYzLC0xNjc5ODg4NjUzLC0yMT
M3NjEyNjU2LC03OTM1OTc4MzcsMTk4MTY0OTc2NSwxNjYyNTgy
MjkxLC0xNjM2NzI3NzI0LC0zNjkzODcxMTIsLTEwNzQ2MzQ1Nz
YsMTI1NzU2NTkyOSwxNDIxNjY5ODIzLDExMTk2MTM3MzcsMTQz
MjAzOTY0MiwtMjMyMzQ2MDM2LDE4NzI4Njg3MzEsMTQ2ODY2MD
Y3OSw2NzA3NjUyODYsLTE0MDg2ODM5NjEsMjgxNzY1NDQ2LC03
NjUwNjc1NDVdfQ==
-->