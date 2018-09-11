# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions or indexes are defined by a name.
This is a 2 dimensional array called *"Sales"* indexed by *"product"* and *"region"*.

`Sales = cp.cube([product, region],[[  1,  2,  3], [ 11, 12, 13], [ 21, 22, 23]])`

In this case the dimension *"product"* is defined as:

    product = cp.index(['Item 1', 'Item 2', 'Item 3'])

and the dimension *"region"* as:

    time = cp.index(['North','South','Center'])

so that the result can be visualized as:
![Sales](https://drive.google.com/open?id=1liAA60Qs972OTNxOFWQohm3muZCr6oVm)

The main goal is providing mathematical operations and functions for easy computing array calculations, leaving to the engine the tasks of realizing array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
Lets suppose we have another cube called:

    Price = cp.cube([product, time], [[ 1, 1.1, 1.2], [ 2, 2.1, 2.2],[ 3, 3.1, 3.2])

Where the *"time"* index is defined as:

    time = cp.index(['2018','2019','2020'])

Then we can calculate *"Revenue"* as follows:

    revenue = Sa


-   individual dimensions (axes) being labeled with meaningful descriptions
-   labeled 'ticks' along each axis
-   indexing and slicing by named axis
-   indexing on any axis with the tick labels instead of only integers
-   reduction operations (like .sum, .mean, etc) support named axis arguments instead of only integer indices.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5MDI3NDIyODYsMTQ2ODY2MDY3OSw2Nz
A3NjUyODYsLTE0MDg2ODM5NjEsMjgxNzY1NDQ2LC03NjUwNjc1
NDUsOTI1ODA5NTg3LDE4ODg4MzY0MTIsLTE2ODg2NTE2ODAsLT
Y1ODA1MzAwMCwxMzkyOTMzODg0LDE2MTk1ODk3NSwxNTQ0MDA2
NDEsLTEyNjc3MDU5NjcsLTI0MzgyMDMyOCwxNDIyMTc0NDA2LC
0xMzAzNDA0NTE4LDQ2NjIyNDI2MCw5MDE1MzgwOTYsMjY4MjE0
NjM2XX0=
-->