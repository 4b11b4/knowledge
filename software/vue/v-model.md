# v-model
https://zaengle.com/blog/using-v-model-on-nested-vue-components
- v-model is nothing more than syntactic sugar for passing a prop to a child
  and then emitting an event
- v-model expects a prop named 'value' and $emits an event when this value
  changes
