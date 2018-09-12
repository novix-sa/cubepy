# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions or indexes are defined by a name.
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
so that the result can be visualized as:
![Sales](https://drive.google.com/file/d/1liAA60Qs972OTNxOFWQohm3muZCr6oVm/view?usp=sharing)

![enter image description here](https://drive.google.com/file/d/1liAA60Qs972OTNxOFWQohm3muZCr6oVm)

The main goal of Cubepy is provide mathematical operations and functions for easy computing array calculations, leaving to the calculation engine the tasks of understanding array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
Lets suppose we have another cube called:

```python
Price = cp.cube([product], [ 1, 2, 3])
```

Then we can calculate *"Revenue"* as follows:

```python
Revenue = Sales * Price
```

In this case the * operations between cubes is interpreted as follows:
For all dimensions that are common to each cube the * mathematical operation is applied element wise. For all dimensions that are not equal the engine broadcast the operation for the not equal index. 
It is easier to interpret the operation with numbers:
(insert graph to explain operation)
![enter image description here](https://drive.google.com/file/d/17D-2mvTpjc4hnDPj1_M_q6OSFHzaIm4r/view?usp=sharing)
## Understanding Array Operations
### Escalar with array
### Equally dimensional arrays
### Operations with arrays of different dimensions
### Operations with arrays and indexes
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2MzY3Mjc3MjQsLTM2OTM4NzExMiwtMT
A3NDYzNDU3NiwxMjU3NTY1OTI5LDE0MjE2Njk4MjMsMTExOTYx
MzczNywxNDMyMDM5NjQyLC0yMzIzNDYwMzYsMTg3Mjg2ODczMS
wxNDY4NjYwNjc5LDY3MDc2NTI4NiwtMTQwODY4Mzk2MSwyODE3
NjU0NDYsLTc2NTA2NzU0NSw5MjU4MDk1ODcsMTg4ODgzNjQxMi
wtMTY4ODY1MTY4MCwtNjU4MDUzMDAwLDEzOTI5MzM4ODQsMTYx
OTU4OTc1XX0=
-->