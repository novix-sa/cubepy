## Getting Started

#### Import cubepy factory:
```python
import cubepy.factory as cp
```
 
#### Create indexes object:
```python
product = cp.index("product",["Product A","Product B"])
year = cp.index("year",[2017,2018,2019,2020])
```

#### Create quantity cube indexes by product
```python
quantity = cp.cube([product],[10,20])
```

#### Create prices cube indexes by product & year, fill with random values
```python
prices = cp.cube([product,year],[[1,2,3,4],[5,6,7,8]] )
```

#### Calculate the sales by product & year
```python
sales = quantity * prices
print(sales)
```

|  |2017|2018|2019|2020|
|--|--|--|--|--|
|Product A|  10|  20|  30|  40|
|Product B|  100|  120|  140| 160|


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkwNjEwMjI4Ml19
-->