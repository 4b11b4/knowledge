## 7 Secret Vue Patterns
### Smarter Watchers
* watchers can be defined as an object
`watch: {
	inputToWatch: {
		handler: 'stringOfFunctionName'
		immediate: true // if need to call when created() 
	}
