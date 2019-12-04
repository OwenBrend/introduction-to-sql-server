## Working with NULL values
A NULL value could mean 'zero' - if something doesn't happen, it can't be logged in a table. However, NULL can also mean 'unknown' or 'missing'. So consider if it is appropriate to replace them in your results. NULL values provide feedback on data quality. If you have NULL values, and you didn't expect to have any, then you have an issue with either how data is captured or how it's entered in the database.

In this exercise, you'll practice filtering for NULL values, excluding them from results, and replacing them with alternative values.

### Instructions 
- Use a shortcut to select all columns from grid. Then filter the results to only include rows where demand_loss_mw is unknown or missing.
- Adapt your code to return rows where demand_loss_mw is not unknown or missing.

### Sample Database
<img src="https://images2.imgbox.com/19/9b/lZ6ICwsF_o.png" alt="image host"/>

### Query given as the solution:

<section>
    <pre><code>-- Retrieve all columns
SELECT* 
FROM 
  grid 
  -- Return only rows where demand_loss_mw is missing or unknown  
WHERE 
  demand_loss_mw is null;
  </code></pre>
  </section>  
  <section>
    <pre><code>-- Retrieve all columns
SELECT*
FROM 
  grid 
  -- Return rows where demand_loss_mw is not missing or unknown   
WHERE 
  demand_loss_mw IS NOT NULL;
  </code></pre>
  </section> 