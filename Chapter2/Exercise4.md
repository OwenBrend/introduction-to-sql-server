## MIN, MAX and AVG
Along with summing and counting, you'll frequently need to find the minimum, maximum, and average of column values. Thankfully, T-SQL has functions you can use to make the task easier!

### Instructions
- Find the minimum value from the affected_customers column, but only for rows where demand_loss_mw has a value. Name the result min_affected_customers.
- Amend the query to return the maximum value from the same column, this time aliasing as max_affected_customers.
- Return the average value from the affected_customers column, this time aliasing as avg_affected_customers.

### Sample Database
<img src="https://images2.imgbox.com/40/4b/5423hVK8_o.png" alt="image host"/>


### Query Giver As The Solutions
<section>
    <pre><code>-- Find the minimum number of affected customers
SELECT 
  MIN(affected_customers) AS min_affected_customers 
FROM 
  grid
-- Only retrieve rows where demand_loss_mw has a value
WHERE
  demand_loss_mw is not NULL;</code></pre>
</section>
<section>
    <pre><code>-- Find the maximum number of affected customers
SELECT 
  MAX(affected_customers) AS max_affected_customers
FROM 
  grid
-- Only retrieve rows where demand_loss_mw has a value
WHERE 
  demand_loss_mw IS NOT NULL;</code></pre>
</section>
<section>
    <pre><code>-- Find the average number of affected customers
SELECT 
  AVG(affected_customers) AS avg_affected_customers 
FROM 
  grid
-- Only retrieve rows where demand_loss_mw has a value
WHERE 
  demand_loss_mw IS NOT NULL;</code></pre>
</section>
