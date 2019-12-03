## Where
You won't usually want to retrieve every row in your database. You'll have specific information you need in order to answer questions from your boss or colleagues.

The WHERE clause is essential for selecting, updating (and deleting!) data from your tables. You'll continue working with the grid dataset for this exercise.

### Instructions
- Select the description and event_year columns.
- Return rows WHERE the description is 'Vandalism'.

### Sample Database
<img src="https://images2.imgbox.com/77/f5/7hI8FN26_o.png" alt="image host"/>

<html>
    <section>
        <pre>
        <code>
        -- Select description and event_year
SELECT 
  description, 
  event_year 
FROM 
  grid 
  -- Filter the results
where 
  description = 'Vandalism';
        </code>
        </pre>
    </section>