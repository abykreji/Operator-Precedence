### Exercise

> Question: 
##### Select people either under 30 or over 50 with an income above 50000 include people that are 50 that are from either Japan or Australia


```python
SELECT firstname, income, age from customers
WHERE income > 50000 AND (age < 30 OR age >= 50)
and (country = 'Japan' OR country = 'Australia')
```



> Question: 
##### What was our total sales in June of 2004 for orders over 100 dollars?


```python
SELECT SUM(totalamount) from orders
WHERE (orderdate >= '2004-06-01' AND orderdate <= '2004-06-30') 
AND totalamount > 100
```