# Chapter 1 SELECTion Box
## Welcome


It's time to begin writing your own queries! In this first coding exercise, you will use SELECT statements to retrieve columns from a database table. You'll be working with the eurovision table, which contains data relating to individual country performance at the Eurovision Song Contest from 1998 to 2012.

### Introductions
- SELECT the country column FROM the eurovision table.
- Amend your query to return the points column instead of the country column.
- Use TOP to change the existing query so that only the first 50 rows are returned.
- Return a list of unique countries using DISTINCT. Give the results an alias of unique_country.

### Sample Database
<selection>
    <img src="D:\semester_3_4\github\images\exp1.PNG" alt= "DataBase"  >
</selection>

### Query given as the solution:
<html>   
    <section>
    <pre><code>
-- SELECT the country column FROM the eurovision table
select country from eurovision</code></pre>
  </section>  
    <section>
    <pre><code>
-- Select the points column
SELECT 
  points 
FROM 
  eurovision;</code></pre>
  </section>  
    <section>
    <pre><code>-- Limit the number of rows returned
SELECT 
  top (50) points 
FROM 
  eurovision;</code></pre>
  </section>  
     <section>
    <pre><code>
    -- Return unique countries and use an alias
SELECT 
  distinct country as unique_country 
FROM 
  eurovision;</code></pre>
  </section>  
</html>


