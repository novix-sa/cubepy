# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions or index are defined by a name.
This is a 3 dimensional array called "Sales".
Sales = cp.cube(


that aims to bring the labeled data power of  [pandas](http://pandas.pydata.org/)  to the physical sciences, by providing N-dimensional variants of the core pandas data structures.

Our goal is to provide a pandas-like and pandas-compatible toolkit for analytics on multi-dimensional arrays, rather than the tabular data for which pandas excels. Our approach adopts the  [Common Data Model](http://www.unidata.ucar.edu/software/thredds/current/netcdf-java/CDM)  for self- describing scientific data in widespread use in the Earth sciences:`xarray.Dataset`  is an in-memory representation of a netCDF file.library intended for opera

ep** is a Pthon 
-   individual dimensions (axes) being labeled with meaningful descriptions
-   labeled 'ticks' along each axis
-   indexing and slicing by named axis
-   indexing on any axis with the tick labels instead of only integers
-   reduction operations (like .sum, .mean, etc) support named axis arguments instead of only integer indices.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjgxNzY1NDQ2LC03NjUwNjc1NDUsOTI1OD
A5NTg3LDE4ODg4MzY0MTIsLTE2ODg2NTE2ODAsLTY1ODA1MzAw
MCwxMzkyOTMzODg0LDE2MTk1ODk3NSwxNTQ0MDA2NDEsLTEyNj
c3MDU5NjcsLTI0MzgyMDMyOCwxNDIyMTc0NDA2LC0xMzAzNDA0
NTE4LDQ2NjIyNDI2MCw5MDE1MzgwOTYsMjY4MjE0NjM2XX0=
-->