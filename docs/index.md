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

The main goal is providing mathematical operations and functions for easy computing array calculations, leaving to the engine the tasks of realizing array dimensions, aligning them for operating and broadcasting the operations on the corresponding dimensions. The following example:



The goal is to provide a complete set of opepandas-like and pandas-compatible toolkit for analytics on multi-dimensional arrays, rather than the tabular data for which pandas excels. Our approach adopts the  [Common Data Model](http://www.unidata.ucar.edu/software/thredds/current/netcdf-java/CDM)  for self- describing scientific data in widespread use in the Earth sciences:`xarray.Dataset`  is an in-memory representation of a netCDF file.library intended for opera

ep** is a Pthon 
-   individual dimensions (axes) being labeled with meaningful descriptions
-   labeled 'ticks' along each axis
-   indexing and slicing by named axis
-   indexing on any axis with the tick labels instead of only integers
-   reduction operations (like .sum, .mean, etc) support named axis arguments instead of only integer indices.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc5NjI2NTU2MiwxNDY4NjYwNjc5LDY3MD
c2NTI4NiwtMTQwODY4Mzk2MSwyODE3NjU0NDYsLTc2NTA2NzU0
NSw5MjU4MDk1ODcsMTg4ODgzNjQxMiwtMTY4ODY1MTY4MCwtNj
U4MDUzMDAwLDEzOTI5MzM4ODQsMTYxOTU4OTc1LDE1NDQwMDY0
MSwtMTI2NzcwNTk2NywtMjQzODIwMzI4LDE0MjIxNzQ0MDYsLT
EzMDM0MDQ1MTgsNDY2MjI0MjYwLDkwMTUzODA5NiwyNjgyMTQ2
MzZdfQ==
-->