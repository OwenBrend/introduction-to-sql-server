## Order by

In this exercise, you'll practice the use of ORDER BY using the grid dataset. It's loaded and waiting for you! It contains a subset of wider publicly available information on US power outages.

Some of the main columns include:

- description: The reason/ cause of the outage.
- nerc_region: The North American Electricity Reliability Corporation was formed to ensure the reliability of the grid and comprises several regional entities).
- demand_loss_mw: How much energy was not transmitted/consumed during the outage.

### Intorductions
- Select description and event_date from grid. Your query should return the first 5 rows, ordered by event_date.
- Modify your code based on the comments provided on the right.

### Sample Database 
<img src="https://images2.imgbox.com/e2/78/qV68Mujo_o.png" alt="image host"/>
### Query given as the solution:

<html>
    <section>
        <pre>
        <code>
        -- Select the first 5 rows from the specified columns
SELECT top 5
  description, 
  event_date 
FROM 
  grid 
order by
    event_date 
        </code>
        </pre>
    </section>
    
   <section>
    <pre><code>-- Select the top 20 rows from description, nerc_region and event_date
SELECT 
  TOP 20 description,
  nerc_region,
  event_date
FROM 
  grid 
  -- Order by nerc_region, affected_customers & event_date
  -- Event_date should be in descending order
ORDER BY
    nerc_region,
    affected_customers,
    event_date desc;
  </code></pre>
  </section>  
</html>