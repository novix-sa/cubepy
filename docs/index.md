# About Cubepy

**Lorem ipsum** dolor sit amet, consectetur adipiscing elit. Praesent elementum commodo pretium. Nullam bibendum congue sapien in ultricies. Pellentesque nec consequat nulla. Vivamus eros nibh, gravida at fringilla gravida, consectetur quis magna. Fusce eu turpis eu sapien viverra fringilla eu at purus. Sed tristique arcu non dui auctor maximus. Praesent eget ante odio. Ut convallis tellus molestie, iaculis leo eget, rhoncus tellus. Suspendisse pharetra aliquet ex sit amet tincidunt. Nullam feugiat sed nulla vel volutpat. docs





### Getting Started

Import cubepy factory:
```python
import cubepy.factory as cp
```
 
Create indexes object:
```python
product = cp.index("product",["Product A","Product B"])
year = cp.index("year",[2017,2018,2019,2020])
```

Create quantity cube indexes by product

```python
quantity = cp.cube([product],[10,20])
```
Create prices cube indexes by product & year, fill with random values

```python
prices = cp.cube([product,year],[[1,2,3,4],[5,6,7,8]] )
```

Calculate the sales by product & year

```python
sales = quantity * prices
print(sales)
```

|  |2017|2018|2019|2020|
|--|--|--|--|--|
|Product A|  10|  20|  30|  40|
|Product B|  100|  120|  140| 160|


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNDk2MDI1MjUsLTY1ODA1MzAwMCwxMz
kyOTMzODg0LDE2MTk1ODk3NSwxNTQ0MDA2NDEsLTEyNjc3MDU5
NjcsLTI0MzgyMDMyOCwxNDIyMTc0NDA2LC0xMzAzNDA0NTE4LD
Q2NjIyNDI2MCw5MDE1MzgwOTYsMjY4MjE0NjM2XX0=
-->