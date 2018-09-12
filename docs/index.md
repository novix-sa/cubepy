# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions or indexes are defined by a name.
This is an example of a 2 dimensional array called *"Sales"* indexed by *"product"* and *"region"*.

`Sales = cp.cube([product, region],[[  1,  2,  3], [ 11, 12, 13], [ 21, 22, 23]])`

In this case the dimension *"product"* is defined as:

    product = cp.index(['Item 1', 'Item 2', 'Item 3'])

and the dimension *"region"* as:

    time = cp.index(['North','South','Center'])

so that the result can be visualized as:
![Sales](https://drive.google.com/open?id=1liAA60Qs972OTNxOFWQohm3muZCr6oVm)

The main goal is providing mathematical operations and functions for easy computing array calculations, leaving to the engine the tasks of realizing array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
Lets suppose we have another cube called:

    Price = cp.cube([product], [ 1, 2, 3])

Then we can calculate *"Revenue"* as follows:

    Revenue = Sales * Price
In this case the * operations between cubes is interpreted as follows:
For all dimensions that are common to each cube the * mathematical operation is applied element wise. For all dimensions that are not equal the engine broadcast the operation for the not equal index. 
It is easier to interpret


-   individual dimensions (axes) being labeled with meaningful descriptions
-   labeled 'ticks' along each axis
-   indexing and slicing by named axis
-   indexing on any axis with the tick labels instead of only integers
-   reduction operations (like .sum, .mean, etc) support named axis arguments instead of only integer indices.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyNjYzNTA3MDYsLTIzMjM0NjAzNiwxOD
cyODY4NzMxLDE0Njg2NjA2NzksNjcwNzY1Mjg2LC0xNDA4Njgz
OTYxLDI4MTc2NTQ0NiwtNzY1MDY3NTQ1LDkyNTgwOTU4NywxOD
g4ODM2NDEyLC0xNjg4NjUxNjgwLC02NTgwNTMwMDAsMTM5Mjkz
Mzg4NCwxNjE5NTg5NzUsMTU0NDAwNjQxLC0xMjY3NzA1OTY3LC
0yNDM4MjAzMjgsMTQyMjE3NDQwNiwtMTMwMzQwNDUxOCw0NjYy
MjQyNjBdfQ==
-->