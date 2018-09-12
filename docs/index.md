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

![enter image description here](https://drive.google.com/file/d/1liAA60Qs972OTNxOFWQohm3muZCr6oVm)

The main goal of Cubepy is provide mathematical operations and functions for easy computing array calculations, leaving to the calculation engine the tasks of understanding array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
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
### Operations with arrays of different dimensions
### Operations with arrays and indexes
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwNzQ2MzQ1NzYsMTI1NzU2NTkyOSwxND
IxNjY5ODIzLDExMTk2MTM3MzcsMTQzMjAzOTY0MiwtMjMyMzQ2
MDM2LDE4NzI4Njg3MzEsMTQ2ODY2MDY3OSw2NzA3NjUyODYsLT
E0MDg2ODM5NjEsMjgxNzY1NDQ2LC03NjUwNjc1NDUsOTI1ODA5
NTg3LDE4ODg4MzY0MTIsLTE2ODg2NTE2ODAsLTY1ODA1MzAwMC
wxMzkyOTMzODg0LDE2MTk1ODk3NSwxNTQ0MDA2NDEsLTEyNjc3
MDU5NjddfQ==
-->