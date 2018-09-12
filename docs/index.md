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
For all dimensions that are common to each cube the * mathematical operation is applied element wise. For all dimensions that are not equal the engine broadcast the operation for the not equal index. The result dimensions is the union 
It is easier to interpret the operation with numbers:
(insert graph to explain operation)
![enter image description here](https://drive.google.com/file/d/17D-2mvTpjc4hnDPj1_M_q6OSFHzaIm4r/view?usp=sharing)
## Understanding Array Operations
### Escalar with array
### Equally dimensional arrays
### Operations with arrays of different dimensions
### Operations with arrays and indexes
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY2MjU4MjI5MSwtMTYzNjcyNzcyNCwtMz
Y5Mzg3MTEyLC0xMDc0NjM0NTc2LDEyNTc1NjU5MjksMTQyMTY2
OTgyMywxMTE5NjEzNzM3LDE0MzIwMzk2NDIsLTIzMjM0NjAzNi
wxODcyODY4NzMxLDE0Njg2NjA2NzksNjcwNzY1Mjg2LC0xNDA4
NjgzOTYxLDI4MTc2NTQ0NiwtNzY1MDY3NTQ1LDkyNTgwOTU4Ny
wxODg4ODM2NDEyLC0xNjg4NjUxNjgwLC02NTgwNTMwMDAsMTM5
MjkzMzg4NF19
-->