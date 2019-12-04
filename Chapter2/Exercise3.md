## Counting
Having explored the 'MRO' region, let's now explore the 'RFC' region in more detail while learning how to use the COUNT aggregate function.

### Instructions
- Return the COUNT of the grid_id column, aliasing the result as grid_total
- Make the count more meaningful by restricting it to records where the nerc_region is 'RFC'. Name the result RFC_count.

### Sample Database
<img src="https://images2.imgbox.com/f2/8d/ERESbUrt_o.png" alt="image host"/>


### Query Given As The Solutions
<section>
    <pre><code>
    -- Obtain a count of 'grid_id'
SELECT 
  count(grid_id) as grid_total 
FROM 
  grid;
    </code></pre>
</section>
