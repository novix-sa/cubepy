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


Cube((Index('product', ['Product A' 'Product B']),), [20 50])

In [ ]:

### Create prices cube indexes by product & year, fill with random values

In [7]:

prices = cp.cube([year,product],cp.random)

prices

print("asdasdasdad")

asdasdasdad

### Calculate the sales by product & year[](http://localhost:8888/notebooks/Test%20Cubepy.ipynb#Calculate-the-sales-by-product-&-year)

In [6]:

sales = quantity * prices

sales

Out[6]:

Cube((Index('product', ['Product A' 'Product B']), Index('year', [2017 2018 2019 2020])), [[ 940  380  240    0]
 [ 650 2750 4900 2550]])

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2NTg0NzA0ODksMTU0NDAwNjQxLC0xMj
Y3NzA1OTY3LC0yNDM4MjAzMjgsMTQyMjE3NDQwNiwtMTMwMzQw
NDUxOCw0NjYyMjQyNjAsOTAxNTM4MDk2LDI2ODIxNDYzNl19
-->