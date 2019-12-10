## Insert
This exercise consists of two parts: In the first, you'll create a new table very similar to the one you created in the previous interactive exercise. After that, you'll insert some data and retrieve it.

You'll continue working with the Chinook database here.

### Intructions 
- Create a table called tracks with 2 VARCHAR columns named track and album, and one integer column named track_length_mins. Then, select all columns from the new table using the * notation.
- Insert the track 'Basket Case', from the album 'Dookie', with a track length of 3, into the appropriate columns.

### Query Given As The Solution 
<section>
    <pre><code>
    -- Create the table
CREATE TABLE tracks(
	-- Create track column
	track varchar(200),
    -- Create album column
  	album varchar(160),
	-- Create track_length_mins column
	track_length_mins int
);
-- Select all columns from the new table
SELECT 
  * 
FROM 
  tracks;
    </code></pre>
</section>