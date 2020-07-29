## Query 2
## Aggregation

These query were related to Monthly data and i used Extratct Function to pull out monthly data,

AS follows :-

''' 
Select Extract (Month from created) As Month, Count(*),sum (amount),avg(amount)
From loans

GROUP BY Month

ORDER BY Month asc;
'''
