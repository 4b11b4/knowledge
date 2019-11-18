# Custom Options Functions
- It's possible to write a custom function to set options based on the chart
  data. Options functions are passed a `context` object which contains info
  about the chart.
- For example, you could inspect chart data from the `context` object and set
  the chart color based on the average of the values. The function simply
  returns the value for the option that you would usually set manually.
