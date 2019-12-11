## Delete
You may not have permissions to delete from your database, but it is safe to practice it here in this course!

Remember - there is no confirmation before deleting. When you execute the statement, the record(s) are deleted immediately. Always ensure you test with a SELECT and WHERE in a separate query to ensure you are selecting and deleting the correct records. If you forget so specify a WHERE condition, you will delete ALL rows from the table.

### Instructions
- Hit 'Submit Answer' to run the query and view the existing data.
- DELETE the record from album where album_id is 1 and then hit 'Submit Answer'.

### Query Given As The Solution
<section>
    <pre><code>
    -- Run the query
SELECT* 
FROM 
  album
    </code></pre>
</section>
<section>
    <pre><code>
    -- Run the query
SELECT* FROM 
  album 
  -- DELETE the record
delete FROM 
  album 
WHERE 
  album_id= 1 
  -- Run the query again
SELECT* 
FROM 
  album;
    </code></pre>
</section>

