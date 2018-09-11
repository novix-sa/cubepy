# About Cubepy

**Cubepy** is a Python package intended for operating with multidimensional labeled arrays. A labeled array is an array which dimensions are


that aims to bring the labeled data power of  [pandas](http://pandas.pydata.org/)  to the physical sciences, by providing N-dimensional variants of the core pandas data structures.

Our goal is to provide a pandas-like and pandas-compatible toolkit for analytics on multi-dimensional arrays, rather than the tabular data for which pandas excels. Our approach adopts the  [Common Data Model](http://www.unidata.ucar.edu/software/thredds/current/netcdf-java/CDM)  for self- describing scientific data in widespread use in the Earth sciences:`xarray.Dataset`  is an in-memory representation of a netCDF file.library intended for opera

ep** is a Pthon 
-   individual dimensions (axes) being labeled with meaningful descriptions
-   labeled 'ticks' along each axis
-   indexing and slicing by named axis
-   indexing on any axis with the tick labels instead of only integers
-   reduction operations (like .sum, .mean, etc) support named axis arguments instead of only integer indices.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc2NTA2NzU0NSw5MjU4MDk1ODcsMTg4OD
gzNjQxMiwtMTY4ODY1MTY4MCwtNjU4MDUzMDAwLDEzOTI5MzM4
ODQsMTYxOTU4OTc1LDE1NDQwMDY0MSwtMTI2NzcwNTk2NywtMj
QzODIwMzI4LDE0MjIxNzQ0MDYsLTEzMDM0MDQ1MTgsNDY2MjI0
MjYwLDkwMTUzODA5NiwyNjgyMTQ2MzZdfQ==
-->