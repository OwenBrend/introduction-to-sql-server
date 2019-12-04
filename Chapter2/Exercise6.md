## LEN'gth of a string
Knowing the length of a string is key to being able to manipulate it further using other functions, so what better way to start the lesson?

### Introductions 
- Retrieve the length of the description column, returning the results as description_length.

### Sample Database
<img src="https://images2.imgbox.com/5c/f7/ebQHFNEl_o.png" alt="image host"/>


### Query Given As The Solutions
<section>
    <pre><code>
    -- Calculate the length of the description column
SELECT 
  len (description) AS description_length
FROM 
  grid;</code></pre>
</section>