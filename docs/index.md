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

The main goal of the calculation engine is providing mathematical operations and functions for easy computing array calculations, leaving to the engine the tasks of realizing array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example illustrates this concept.
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
eyJoaXN0b3J5IjpbNDUwMDc4NjA4LDE0MjE2Njk4MjMsMTExOT
YxMzczNywxNDMyMDM5NjQyLC0yMzIzNDYwMzYsMTg3Mjg2ODcz
MSwxNDY4NjYwNjc5LDY3MDc2NTI4NiwtMTQwODY4Mzk2MSwyOD
E3NjU0NDYsLTc2NTA2NzU0NSw5MjU4MDk1ODcsMTg4ODgzNjQx
MiwtMTY4ODY1MTY4MCwtNjU4MDUzMDAwLDEzOTI5MzM4ODQsMT
YxOTU4OTc1LDE1NDQwMDY0MSwtMTI2NzcwNTk2NywtMjQzODIw
MzI4XX0=
-->