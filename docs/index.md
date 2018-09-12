# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions or indexes are defined by a name.
This is an example of a 2 dimensional array called *"Sales"* indexed by *"product"* and *"region"*.

`Sales = cp.cube([product, region],[[  1,  2,  3], [ 11, 12, 13], [ 21, 22, 23]])`

In this case the dimension *"product"* is defined as:

    product = cp.index(['Item 1', 'Item 2', 'Item 3'])

and the dimension *"region"* as:

    time = cp.index(['North','South','Center'])

so that the result can be visualized as:
![Sales](https://drive.google.com/file/d/1liAA60Qs972OTNxOFWQohm3muZCr6oVm/view?usp=sharing)

The main goal is providing mathematical operations and functions for easy computing array calculations, leaving to the engine the tasks of realizing array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
Lets suppose we have another cube called:

    Price = cp.cube([product], [ 1, 2, 3])

Then we can calculate *"Revenue"* as follows:

    Revenue = Sales * Price
In this case the * operations between cubes is interpreted as follows:
For all dimensions that are common to each cube the * mathematical operation is applied element wise. For all dimensions that are not equal the engine broadcast the operation for the not equal index. 
It is easier to interpret the operation with numbers:
(insert graph to explain operation)
![enter image description here](https://drive.google.com/file/d/17D-2mvTpjc4hnDPj1_M_q6OSFHzaIm4r/view?usp=sharing)
## Understanding Array Operations
### Escalar with array
### Equally dimensional arrays
### Operations arrays with different dimensions
### Operations with arrays and indexes
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTU4MDk5MzY4MCwxMTE5NjEzNzM3LDE0Mz
IwMzk2NDIsLTIzMjM0NjAzNiwxODcyODY4NzMxLDE0Njg2NjA2
NzksNjcwNzY1Mjg2LC0xNDA4NjgzOTYxLDI4MTc2NTQ0NiwtNz
Y1MDY3NTQ1LDkyNTgwOTU4NywxODg4ODM2NDEyLC0xNjg4NjUx
NjgwLC02NTgwNTMwMDAsMTM5MjkzMzg4NCwxNjE5NTg5NzUsMT
U0NDAwNjQxLC0xMjY3NzA1OTY3LC0yNDM4MjAzMjgsMTQyMjE3
NDQwNl19
-->