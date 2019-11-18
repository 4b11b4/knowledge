# Display vs Render
https://www.chartjs.org/docs/latest/general/responsive.html
- It will be necessary to have the chart size be able to dynamically adjust to
  the window size.
- It is not possible to set the `<canvas>` element to have a
  relative width or height. For example, you cannot write:
  `<canvas height="40vh">`. The canvas will not resize.
- Responsive re-sizing can be enabled by setting the `responsive`
  configuration option to `true`.
  - You must put the canvas in a `<div>` in order for responsive re-sizing to
    occur. The div must contain the chart element and nothing else.
    e.g. `<div class="chart-container" style="position: relative;">`
