## Assignment 5: Web Analytics Dashboard

### CSV & PapaParse

Data is stored in a CSV file, which is a plain text file with commas between rows and columns. PapaParse imports the `data.csv` file for this project and parses information into JavaScript objects, giving each row attributes such as sessions, income, and source. Instead of reading raw text, this makes it simple to work with the data in JavaScript. Calculations like totals and averages may be performed accurately since the `dynamicTyping: true` option automatically transforms numeric values from strings into actual numbers.

### KPI Calculation

Because `.reduce()` goes through the array and maintains a running total, I utilized it to determine the KPI values. Each row adds its values to the totals, which are stored in the accumulator. Because of this, it can be used to aggregate data in a single pass, such as total sessions, revenue, and pageviews. Additionally, I calculated the average bounce rate and conversion rate using the results from `.reduce()`, which maintains all KPI computations based on the CSV data.

### Chart Types

Because bar charts work well for comparing categories side by side, I utilized them to compare sessions or income across traffic sources. Since a doughnut chart makes it obvious how much each source adds to the total, I used it to illustrate revenue share. Because a line chart makes it simple to see trends across months, I used it to display sessions across time. The dashboard is easier to grasp because each chart style corresponds to the type of data being displayed.

### Real-World Reflection

The data displays the performance of different traffic sources in terms of income, conversions, and sessions. While some sources may increase traffic, others may increase revenue or improve conversion rates. A source with a high session count, for instance, might not always have the highest revenue, indicating variations in performance. By highlighting the most useful sources and where to concentrate content or marketing efforts, this dashboard assists a news editor in making judgments.
