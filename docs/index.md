# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions or index are defined by a name.
This is a 2 dimensional array called *"Sales"* indexed by *"product"* and *"region"*.

`Sales = cp.cube([product, region],[[  1,  2,  3], [ 11, 12, 13], [ 21, 22, 23]])`

In this case the dimension *"product"* is defined as:

    product = cp.index(['Item 1', 'Item 2', 'Item 3'])
and the dimension *"region"* as:

    time = cp.index(['North','South','Center'])

so that the result can be visualized as:


that aims to bring the labeled data power of  [pandas](http://pandas.pydata.org/)  to the physical sciences, by providing N-dimensional variants of the core pandas data structures.

Our goal is to provide a pandas-like and pandas-compatible toolkit for analytics on multi-dimensional arrays, rather than the tabular data for which pandas excels. Our approach adopts the  [Common Data Model](http://www.unidata.ucar.edu/software/thredds/current/netcdf-java/CDM)  for self- describing scientific data in widespread use in the Earth sciences:`xarray.Dataset`  is an in-memory representation of a netCDF file.library intended for opera

ep** is a Pthon 
-   individual dimensions (axes) being labeled with meaningful descriptions
-   labeled 'ticks' along each axis
-   indexing and slicing by named axis
-   indexing on any axis with the tick labels instead of only integers
-   reduction operations (like .sum, .mean, etc) support named axis arguments instead of only integer indices.
<!--stackedit_data:
eyJoaXN0b3J5IjpbNjcwNzY1Mjg2LC0xNDA4NjgzOTYxLDI4MT
c2NTQ0NiwtNzY1MDY3NTQ1LDkyNTgwOTU4NywxODg4ODM2NDEy
LC0xNjg4NjUxNjgwLC02NTgwNTMwMDAsMTM5MjkzMzg4NCwxNj
E5NTg5NzUsMTU0NDAwNjQxLC0xMjY3NzA1OTY3LC0yNDM4MjAz
MjgsMTQyMjE3NDQwNiwtMTMwMzQwNDUxOCw0NjYyMjQyNjAsOT
AxNTM4MDk2LDI2ODIxNDYzNl19
-->