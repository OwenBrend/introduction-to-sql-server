## Inner Join (II)
Here, you'll continue to practice your INNER JOIN skills. We'll use the album table as last time, but will join it to a new table - artist - which consists of two columns: artist_id and name.

### Instructions
- Select the album_id and title columns from album (the main source table name).
- Select the name column from artist and alias it as artist.
- Identify a common column between the album and artist tables and perform an inner join.

### Sample Database

### Query Given As The Solution
<section>
    <pre><code>-- Select album_id and title from album, and name from artist
SELECT 
  album.album_id,
  album.title,
  name AS artist
  -- Enter the main source table name
FROM album
  -- Perform the inner join
INNER JOIN artist on artist.artist_id = album.artist_id;
    </code></pre>
</section>