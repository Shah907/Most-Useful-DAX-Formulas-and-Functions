# 51 Most Useful DAX Formulas and Functions


<!-- wp:paragraph -->
<p>DAX stands for Data Analysis Expressions. It's a formula and query language used in Microsoft Power BI, Power Pivot, and Analysis Services Tabular projects. DAX is designed to work with tables and columns, much like Excel formulas, but it's optimized for handling large volumes of data and performing complex calculations.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>With DAX, you can create calculated columns, tables, and measures to perform various types of data analysis, such as aggregations, comparisons, and statistical calculations. It's widely used in business intelligence and analytics to derive insights from data and create interactive visualizations.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 class="wp-block-heading" id="h-51-most-useful-dax-data-analysis-expressions-formulas">51 Most Useful DAX (Data Analysis Expressions) Formulas</h2>
<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-1-sum">1. SUM</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Calculates the sum of values in a column or expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales = SUM(Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the total sales amount from the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-2-average">2. AVERAGE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Calculates the average of values in a column or expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Average Sales = AVERAGE(Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the average sales amount from the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-3-count">3. COUNT</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Counts the number of rows in a table or the number of values in a column.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Customers = COUNT(Customers[CustomerID])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Counts the total number of customers in the 'Customers' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-4-max">4. MAX</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the maximum value from a column or expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Highest Sales = MAX(Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Find the highest sales amount from the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-5-min">5. MIN</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the minimum value from a column or expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Lowest Sales = MIN(Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Finds the lowest sales amount from the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-6-distinct">6. DISTINCT</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a one-column table containing unique values from a column or table expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Unique Customers = DISTINCT(Sales[CustomerID])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns a list of unique customer IDs from the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-7-related">7. RELATED</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a related value from another table.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Customer Country = RELATED(Customers[Country])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Retrieves the country associated with a customer from the 'Customers' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-8-filter">8. FILTER</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a table that has been filtered based on specified criteria.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>High Value Sales = FILTER(Sales, Sales[Amount] &gt; 1000)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Filters the 'Sales' table to include only sales with amounts greater than 1000.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-9-calculate">9. CALCULATE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Evaluates an expression in a modified filter context.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales 2019 = CALCULATE(SUM(Sales[Amount]), 'Calendar'[Year] = 2019)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the total sales amount for the year 2019.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-10-all">10. ALL</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns all the rows in a table, or all the values in a column, ignoring any filters that might have been applied.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales (All) = CALCULATE(SUM(Sales[Amount]), ALL(Sales))</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the total sales amount regardless of any filters applied to the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-11-distinctcount">11. DISTINCTCOUNT</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the count of distinct values in a column.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Unique Customers Count = DISTINCTCOUNT(Sales[CustomerID])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Counts the number of unique customers in the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-12-concatenatex">12. CONCATENATEX</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Concatenates the result of an expression evaluated for each row in a table, using a specified delimiter.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Customer List = CONCATENATEX(Customers, Customers[Name], &quot;, &quot;)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Creates a comma-separated list of customer names from the 'Customers' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-13-sumx">13. SUMX</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Iterates over each row in a table, evaluates an expression, and returns the sum of the results.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales (SumX) = SUMX(Sales, Sales[Quantity] * Sales[UnitPrice])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the total sales amount by multiplying quantity with unit price for each row and summing the results.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-14-averagex">14. AVERAGEX</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Iterates over each row in a table, evaluates an expression, and returns the average of the results.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Average Sales (AvgX) = AVERAGEX(Sales, Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the average sales amount for each row in the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-15-countrows">15. COUNTROWS</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Counts the number of rows in a table or table expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Orders = COUNTROWS(Orders)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Counts the total number of orders in the 'Orders' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-16-divide">16. DIVIDE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Divides two numbers and handles errors gracefully by returning a specified alternate result.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Sales Conversion Rate = DIVIDE(COUNT(Sales[Converted]), COUNT(Sales[Visitors]), 0)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the conversion rate of visitors to converted sales, handling division by zero errors.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-17-blank">17. BLANK</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a blank value.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Missing Sales = IF(ISBLANK([Total Sales]), &quot;No sales data available&quot;, [Total Sales])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Displays a message if total sales data is missing.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-18-date">18. DATE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Creates a date from the specified year, month, and day.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Date = DATE(2022, 4, 15)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Creates a date for April 15, 2022.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-19-calculatetable">19. CALCULATETABLE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Evaluates an expression over a table, with the option to modify the filter context.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Top Customers = CALCULATETABLE('Customers', 'Customers'[Total Purchases] &gt; 1000)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns a table of customers with total purchases exceeding 1000.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-20-distinctcountnoblank">20. DISTINCTCOUNTNOBLANK</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the count of distinct non-blank values in a column.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Unique Products Sold = DISTINCTCOUNTNOBLANK(Sales[ProductID])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Counts the number of unique products sold, excluding any blank product IDs.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-21-earlier">21. EARLIER</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the value of a column from the previous row in the current context.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Sales Growth = Sales[Amount] - EARLIER(Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the sales growth compared to the previous row.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-22-rankx">22. RANKX</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the rank of a value in a column, optionally based on a specified expression and order.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Sales Rank = RANKX(Sales, Sales[Amount])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the rank of sales amounts in the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-23-percentilex-inc">23. PERCENTILEX.INC</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the nth percentile of values in a column, inclusive of the nth percentile value.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>90th Percentile Sales = PERCENTILEX.INC(Sales, Sales[Amount], 0.9)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the 90th percentile sales amount in the 'Sales' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-24-switch">24. SWITCH</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Evaluates a list of conditions and returns the result corresponding to the first true condition.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Sales Category = SWITCH(TRUE(),

 [Total Sales] &gt; 10000, &quot;High&quot;, [Total Sales] &gt; 5000, &quot;Medium&quot;, &quot;Low&quot;)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Categorizes sales into "High", "Medium", or "Low" based on their total amount.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-25-userelationship">25. USERELATIONSHIP</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Specifies a relationship to be used in a calculation, overriding the active relationship.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Sales Amount (Alternate Date) = CALCULATE(SUM(Sales[Amount]), USERELATIONSHIP(Sales[Date], 'AlternateDate'[Date]))</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the sales amount using an alternate date relationship.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-26-lookupvalue">26. LOOKUPVALUE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the value of a column from a single row that meets the specified criteria.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Customer Name = LOOKUPVALUE(Customers[Name], Customers[CustomerID], 123)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the name of the customer with the ID 123.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-27-relatedtable">27. RELATEDTABLE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a table related to the current table by a foreign key relationship.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Customer Orders = RELATEDTABLE(Orders)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns all orders related to the current customer.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-28-removefilters">28. REMOVEFILTERS</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Removes all filters from the specified columns or tables.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales (No Filters) = CALCULATE(SUM(Sales[Amount]), REMOVEFILTERS())</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the total sales amount without any filters applied.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-29-selectcolumns">29. SELECTCOLUMNS</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a table with selected columns from another table.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Customer Names = SELECTCOLUMNS(Customers, &quot;Name&quot;, Customers[Name])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns a table with only the "Name" column from the 'Customers' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-30-addcolumns">30. ADDCOLUMNS</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a table with additional calculated columns.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Customer Profitability = ADDCOLUMNS(Customers, &quot;Profit&quot;, [Total Sales] - [Total Costs])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Adds a "Profit" column to the 'Customers' table calculated as total sales minus total costs.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-31-coalesce">31. COALESCE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the first non-blank value from a list of expressions.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Preferred Language = COALESCE(User[PreferredLanguage], &quot;English&quot;)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the preferred language of the user or defaults to English if not specified.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-32-relatedtable">32. RELATEDTABLE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns a table related to the current table by a foreign key relationship.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Product Sales = RELATEDTABLE(Sales)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns all sales related to the current product.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-33-isfiltered">33. ISFILTERED</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Checks if a column or table has been filtered.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Is Date Filtered = ISFILTERED('Calendar'[Date])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Checks if the date column has been filtered.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-34-firstdate">34. FIRSTDATE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the earliest date from a column containing dates.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>First Order Date = FIRSTDATE(Orders[OrderDate])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the date of the first order in the 'Orders' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-35-lastdate">35. LASTDATE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the latest date from a column containing dates.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Last Order Date = LASTDATE(Orders[OrderDate])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the date of the last order in the 'Orders' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-36-dateadd">36. DATEADD</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Adds or subtracts a specified number of units to a date.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Next Month = DATEADD('Calendar'[Date], 1, MONTH)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the date one month after the specified date.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-37-datediff">37. DATEDIFF</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Calculates the difference between two dates.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Days Between Orders = DATEDIFF(Orders[OrderDate], Orders[PreviousOrderDate], DAY)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the number of days between consecutive orders.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-38-totalytd">38. TOTALYTD</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Calculates a year-to-date total for a specified expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales YTD = TOTALYTD(SUM(Sales[Amount]), 'Calendar'[Date])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the year-to-date total sales amount.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-39-totalmtd">39. TOTALMTD</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Calculates a month-to-date total for a specified expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Total Sales MTD = TOTALMTD(SUM(Sales[Amount]), 'Calendar'[Date])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Calculates the month-to-date total sales amount.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-40-firstnonblank">40. FIRSTNONBLANK</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the first non-blank value from a column, optionally evaluating an expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>First Sale Amount = FIRSTNONBLANK(Sales[Amount], 0)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the first non-blank sales amount or 0 if no value is found.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-41-lastnonblank">41. LASTNONBLANK</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the last non-blank value from a column, optionally evaluating an expression.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Last Sale Amount = LASTNONBLANK(Sales[Amount], 0)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the last non-blank sales amount or 0 if no value is found.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-42-selectedvalue">42. SELECTEDVALUE</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the single value in a column when there's only one value, otherwise returns a default value.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Selected Product = SELECTEDVALUE(Products[ProductID], &quot;Multiple Products&quot;)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the selected product ID or "Multiple Products" if more than one product is selected.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-43-username">43. USERNAME</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the username of the current user.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Current User = USERNAME()</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the username of the current user.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-44-userprincipalname">44. USERPRINCIPALNAME</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the user principal name (UPN) of the current user.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Current User UPN = USERPRINCIPALNAME()</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the user principal name (email address) of the current user.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-45-username">45. USERNAME</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the username of the current user.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Current User = USERNAME()</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the username of the current user.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-46-earliest">46. EARLIEST</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the earliest date among a set of dates.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Earliest Date = EARLIEST('Calendar'[Date1], 'Calendar'[Date2], 'Calendar'[Date3])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the earliest date among Date1, Date2, and Date3.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-47-latest">47. LATEST</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the latest date among a set of dates.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Latest Date = LATEST('Calendar'[Date1], 'Calendar'[Date2], 'Calendar'[Date3])</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the latest date among Date1, Date2, and Date3.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-48-contains">48. CONTAINS</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Checks if a table or column contains a specific value.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Has High Sales = CONTAINS(Sales, Sales[Amount], 1000)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Checks if the 'Sales' table contains any sales with an amount of 1000.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-49-pathcontains">49. PATHCONTAINS</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Checks if a path contains a specific value.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Has Path = PATHCONTAINS('Paths', &quot;PathName&quot;, &quot;Value&quot;)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Checks if the 'Paths' table contains the specified value in the "PathName" column.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-50-pathlength">50. PATHLENGTH</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the length of a path.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Path Length = PATHLENGTH('Paths', &quot;PathName&quot;)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the length of the path specified in the "PathName" column of the 'Paths' table.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading" id="h-51-pathitem">51. PATHITEM</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Description:</strong> Returns the nth item in a path.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example:</strong></p>
<!-- /wp:paragraph -->

<!-- wp:codemirror-blocks/code-block {"mode":"sql","mime":"text/x-sql"} -->
<div class="wp-block-codemirror-blocks-code-block code-block"><pre>Path Item = PATHITEM('Paths', &quot;PathName&quot;, 2)</pre></div>
<!-- /wp:codemirror-blocks/code-block -->

<!-- wp:paragraph -->
<p>Returns the second item in the path specified in the "PathName" column of the 'Paths' table.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>These DAX formulas cover various functionalities commonly used in Power BI and other analysis tools for manipulating and analyzing data.</p>
<!-- /wp:paragraph -->
