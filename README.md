# Umba-Product-analyst

Solving SQL query's.

  - Joining table

'''
Select transactions.loan_id, loans.amount, loans.user_id, users.created, transactions.transaction_fee, transactions.t_type
from loans inner join transactions on loans.user_id = transactions.user_id
inner join users on transactions.user_id = users.id
where loan_status = 'repaid' and t_type = 'disbursement' 
order by created '''

**By running this query**

We will get the table which shows the number of loans withdrawn for the transaction of type disbursement .
