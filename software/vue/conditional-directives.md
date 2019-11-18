# Conditional Directives
Conditional directives provide the ability to show or hide elements. Vue
provides four "directives" to achieve this:
1. `v-if`
- adds or removes DOM elements based on the given expression
2. `v-else`
- must be in an element that comes immediately after a `v-if` or `v-else-if`
3. `v-else-if`
- when you need more than two options
4. `v-show`
- similar to `v-if`, but:
  `v-show` renders all elements to the DOM and then uses CSS *display*
  property to hide elements if the expression is false
- does not support `v-else`

notes:
- `v-show` has a performance advantage if the elements are switched frequently
- `v-if` has the advantage for initial render time
