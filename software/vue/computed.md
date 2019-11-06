# Asynchronous Action Inside A Computed Property
- Vue does not allow commands such as axios.get() inside a computed property
  definition, as this simply doesn't make sense for the specific use case of
  a computed property.
