## Exploring classic rock songs - AND/OR
Having familiarized yourself with the songlist table, you'll now extend your WHERE clause from the previous exercise.

### Instructions
- Extend the WHERE clause so that the results are those with a release_year greater than or equal to 1980 and less than or equal to 1990.
- Update your query to use an OR instead of an AND.

### Sample Database
<img src="https://images2.imgbox.com/0f/b5/nOkLvXFc_o.png" alt="image host"/>

### Query Given As The Solutions
<section>
    <pre><code>SELECT 
  song, 
  artist, 
  release_year
FROM 
  songlist 
WHERE 
  -- Retrieve records greater than and including 1980
  release_year >= 1980 
  -- Also retrieve records up to and including 1990
  and release_year <= 1990 
ORDER BY 
  artist, 
  release_year;
  </code></pre>
  </section>  
    <section>
    <pre><code>SELECT 
  song, 
  artist, 
  release_year
FROM 
  songlist 
WHERE 
  -- Retrieve records greater than and including 1980
  release_year >= 1980 
  -- Replace AND with OR
  OR release_year <= 1990 
ORDER BY 
  artist, 
  release_year;
  </code></pre>
  </section>  