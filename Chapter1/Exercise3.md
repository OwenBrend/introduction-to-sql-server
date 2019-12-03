## More selections

Now that you've practiced how to select one column at a time, it's time to practice selecting more than one column. You'll continue working with the eurovision table.

### Introductions
- SELECT the country and event_year columns from the eurovision table.
- Use a shortcut to amend the current query, returning ALL rows from ALL columns in the table.
- Return all columns, but only include the top half of the table - in other words, return 50 percent of the rows.

### Sample Database
<img src="https://images2.imgbox.com/25/53/Rp2ebNfq_o.png" alt="image host"/>

### Query given as the solution:
<html>
    <section>
        <pre>
            <code>
            -- Select country and event_year from eurovision
select
  country, 
  event_year 
from 
  eurovision;
            </code>
        </pre>
    </section>
    <section>
    <pre>
    <code>
    -- Amend the code to select all rows and columns
select*from eurovision;
    </code>
    </pre>
    </section>
    
    <section>
    <pre>
    <code>
   -- Return all columns, restricting the percent of rows returned
SELECT TOP 50 PERCENT * FROM eurovision;
    </code>
    </pre>
    </section>
</html>
