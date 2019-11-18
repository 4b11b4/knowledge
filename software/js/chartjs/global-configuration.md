# Global Chart Configuration
https://www.chartjs.org/docs/latest/configuration/
- This was introduced in order to keep chart configuration `DRY` (i.e. do not
  repeat yourself).
- For example, you can turn off lines for all datasets by default, but then
  override them individually if you need to.
  `Chart.defaults.global.datasets.line.showLine = false;`
  - Note that the line above only affects plots of type `line` and does not
    affect other charts such as `scatter`.
