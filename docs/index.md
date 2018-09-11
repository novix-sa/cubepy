# About Cubepy

**Lorem ipsum** dolor sit amet, consectetur adipiscing elit. Praesent elementum commodo pretium. Nullam bibendum congue sapien in ultricies. Pellentesque nec consequat nulla. Vivamus eros nibh, gravida at fringilla gravida, consectetur quis magna. Fusce eu turpis eu sapien viverra fringilla eu at purus. Sed tristique arcu non dui auctor maximus. Praesent eget ante odio. Ut convallis tellus molestie, iaculis leo eget, rhoncus tellus. Suspendisse pharetra aliquet ex sit amet tincidunt. Nullam feugiat sed nulla vel volutpat. docs


### Installing Cubepy

Install the  `cubepy`  package using pip:
```
pip install cubepy
```


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
quantity = cp.cube([product],[20,50,30])
```
Create prices cube indexes by product & year, fill with random values

```python
prices = cp.cube([year,product],cp.random)
```

Calculate the sales by product & year

```python
sales = quantity * prices
print(sales)
```

|  |2017|2018|2019|2020|
|--|--|--|--|--|
|Product A|  940|  380|  240|  0|
|Product B|  650|  2750|  4900| 2550|


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYxOTU4OTc1LDE1NDQwMDY0MSwtMTI2Nz
cwNTk2NywtMjQzODIwMzI4LDE0MjIxNzQ0MDYsLTEzMDM0MDQ1
MTgsNDY2MjI0MjYwLDkwMTUzODA5NiwyNjgyMTQ2MzZdfQ==
-->