## Assignment 5: Web Analytics Dashboard

### CSV & PapaParse

A CSV file is a plain text file that stores data in rows and columns separated by commas. In this project, PapaParse loads the `data.csv` file and parses it into JavaScript objects, where each row becomes an object with properties like sessions, revenue, and source. This makes the data easy to work with in JavaScript instead of reading raw text. The `dynamicTyping: true` option automatically converts numeric values from strings into actual numbers, which allows calculations like totals and averages to work correctly.

### KPI Calculation

I used `.reduce()` to calculate the KPI values because it loops through the array and keeps a running total. The accumulator stores the totals while each row adds its values to those totals. This makes it useful for aggregating data like total sessions, revenue, and pageviews in one pass. I also used the results from `.reduce()` to calculate average bounce rate and conversion rate, which keeps all KPI calculations based on the CSV data.

### Chart Types

I used a bar chart to compare sessions or revenue across traffic sources because bar charts are good for comparing categories side by side. I used a doughnut chart to show revenue share because it clearly shows how much each source contributes to the total. I used a line chart to show sessions over time because it makes trends across months easy to see. Each chart type matches the type of data being shown, which makes the dashboard easier to understand.

### Real-World Reflection

The data shows how different traffic sources perform across sessions, revenue, and conversions. Some sources may bring in more traffic, while others generate more revenue or better conversion rates. For example, a source with high sessions may not always have the highest revenue, which shows differences in performance. This dashboard helps a news editor make decisions by showing which sources are most valuable and where to focus content or marketing efforts.
