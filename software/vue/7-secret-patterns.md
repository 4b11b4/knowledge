## 7 Secret Vue Patterns
from:
https://www.youtube.com/watch?v=7YZ5DwlLSt8
https://github.com/chrisvfritz/vue-enterprise-boilerplate

### Smarter Watchers
* watchers can be defined as an object
`watch: {
	inputToWatch: {
		handler: 'stringOfFunctionName'
		immediate: true // if need to call when created() 
	}

### Global Component Registration
* for `Base` components, you can import them once instead of individually all over the place

### Global Module (vuex state modules) Registration
* same as above, but useful when you have multiple modules

### Namespaced Modules
* TODO: add more info

### Cleaner Views
* on route changes, can set to re-render always, to prevent bugs

### Transparent Wrapper Components
e.g. `BaseButton` etc.
* listener objects
* inheriting attributes

### Render Functions for Multi-Root Components
* e.g. a component that uses a v-for to render `<li>` for `<router-link>`s
* requires knowing how to write `render` functions
