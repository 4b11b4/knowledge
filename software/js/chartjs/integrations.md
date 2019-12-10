# Integrations
## vue-chartjs
1. Vue.js
  - You can integrate Chart.js into your Vue components with `extends` or
    `mixins`.
  - The vue-chartjs library provides two mixins to enable the chart to update
    if the data object is changed.
  - If you are working with chart data that will be retrieved from an async
    call, it may be wise to use a `v-if` directive to only add the component
    to the DOM if some boolean variable is true (e.g. a flag which is set
    after the data has been retrieved).
