## Declare multiple variables
You've seen how to DECLARE and SET set 1 variable. Now, you'll DECLARE and SET multiple variables. There is already one variable declared, however you need to overwrite this and declare 3 new ones. The WHERE clause will also need to be modified to return results between a range of dates.

### Instructions
- Declare a new variable called @start of type DATE.
- Declare a new variable called @stop of type DATE.
- Declare a new variable called @affected of type INT.
- Retrieve all rows where event_date is BETWEEN @start and @stop and affected_customers is greater than or equal to @affected.

### Query Given As The Solution
<section>
    <pre><code>
    -- Declare @start
declare @start date

-- SET @start to '2014-01-24'
set @start ='2014-01-24'
    </code></pre>
</section>
<section>
    <pre><code>
    -- Declare @start
DECLARE @start DATE

-- Declare @stop
declare @stop date

-- SET @start to '2014-01-24'
SET @start = '2014-01-24'

-- SET @stop to '2014-07-02'
set @stop='2014-07-02'
    </code></pre>
</section>
<section>
    <pre><code>
    -- Declare @start
DECLARE @start DATE

-- Declare @stop
DECLARE @stop DATE

-- Declare @affected
declare @affected INT

-- SET @start to '2014-01-24'
SET @start = '2014-01-24'

-- SET @stop to '2014-07-02'
SET @stop  = '2014-07-02'

-- Set @affected to 5000
set @affected =5000
    </code></pre>
</section>
<section>
    <pre><code>
    -- Declare your variables
DECLARE @start DATE
DECLARE @stop DATE
DECLARE @affected INT;
-- SET the relevant values for each variable
SET @start = '2014-01-24'
SET @stop  = '2014-07-02'
SET @affected =  5000 ;

SELECT 
  description,
  nerc_region,
  demand_loss_mw,
  affected_customers
FROM 
  grid
-- Specify the date range of the event_date and the value for @affected
where event_date between '2014-01-24' AND '2014-07-02'
AND affected_customers >= 12000;
    </code></pre>
</section>