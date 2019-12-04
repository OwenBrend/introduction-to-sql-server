## Exploring classic rock songs
It's time to rock and roll! In this set of exercises, you'll use the songlist table, which contains songs featured on the playlists of 25 classic rock radio stations.

First, let's get familiar with the data.

### Instructions
- Retrieve the song, artist, and release_year columns from the songlist table.
- Make sure there are no NULL values in the release_year column.
- Order the results by artist and release_year.

### Sample Database
<img src="https://images2.imgbox.com/ae/fe/vNEFB54F_o.png" alt="image host"/>

### Query Gives As The Solutions
<section>
    <pre><code>-- Retrieve the song, artist and release_year columns
SELECT
  song, 
  artist, 
  release_year
from
  songlist
  </code></pre>
  </section>  
  <section>
    <pre><code>-- Retrieve the song, artist and release_year columns
SELECT 
  song,
  artist,
  release_year
FROM 
  songlist 
where
 release_year is not null
  </code></pre>
  </section> 
  
  <section>
    <pre><code>-- Retrieve the song,artist and release_year columns
SELECT 
  song, 
  artist, 
  release_year 
FROM 
  songlist 
  -- Ensure there are no missing or unknown values in the release_year column
WHERE 
  release_year IS NOT NULL 
  -- Arrange the results by the artist and release_year columns
order by
  artist, 
  release_year;</code></pre>
  </section> 