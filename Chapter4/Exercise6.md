## Update
You may sometimes have to update the rows in a table. For example, in the album table, there is a row with a very long album title, and you may want to shorten it.

You don't want to delete the record - you just want to update it in place. To do this, you need to specify the album_id to ensure that only the desired row is updated and all others are not modified.

### Intructions
- Select the title column from the album table where the album_id is 213.
- That's a very long album title, isn't it? Use an UPDATE statement to modify the title to 'Pure Cult: The Best Of The Cult'.
- Hit 'Submit Answer' to see whether or not the album title was shortened!

### Query Given As The Solution
<section>
    <pre><code>
    -- Select the album
SELECT 
  title 
FROM 
  album 
WHERE 
  album_id = 213;
    </code></pre>
</section>
<section>
    <pre><code>
    -- Run the query
SELECT 
  title 
FROM 
  album 
WHERE 
  album_id = 213;
-- UPDATE the title of the album
update 
  album
set 
  title = 'Pure Cult: The Best Of The Cult'
WHERE album_id = 213;
    </code></pre>
</section>
<section>
    <pre><code>
    -- Select the album
SELECT 
  title 
FROM 
  album 
WHERE 
  album_id = 213;
-- UPDATE the title of the album
UPDATE 
  album 
SET 
  title = 'Pure Cult: The Best Of The Cult' 
WHERE 
  album_id = 213;
-- Run the query again
SELECT 
  title 
FROM 
  album ;
    </code></pre>
</section>