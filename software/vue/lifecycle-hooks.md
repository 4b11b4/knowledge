# Creation
You can perform actions before the component has been added to the DOM.

1. beforeCreate
- Very first hook run in a component.
- `data` has not been made reactive. `events` have not been set up.

2. created
- You do have access to `data` and `events` do exist.
- Templates and Virtual DOM have not been mounted or rendered.

# Mounting (DOM Insertion)
These are the used most often. They allow you to access the component before
and after the initial render happens. They should be used if the DOM of your
component needs to be modified immediately before or after it is rendered.

Mounted hooks should not be used for server side rendering.

1. beforeMount
- This method is invoked after our template has been compiled and virtual DOM
  updated by Vue.

2. mounted
- After beforeMount, the `$el` property is added to the Vue instance, the
  native DOM is updated, and then mounted() is ran.
- It is mostly used for fetching data for a component and modifying the DOM
  to integrate other libraries and frameworks aside Vue.
- It gives you access to templates and enables interaction with the DOM.

# Updating
Useful for debugging. They are called whenever a reactive property used by a
component changes or re-renders.

You shouldn't use `updating` methods for changing any state though:
computed properties or watchers are better for that.

# Destruction
Allow you to do any cleanup or inform a remote server that a component was
removed.
