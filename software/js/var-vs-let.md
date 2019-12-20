## `var` vs `let`
1. Scope
* immediate function body: `var`
* immediate enclosing block: `let`

2. Declaration
* not accessible until declaration: `let`
```javascript
function checkHoisting() {
	console.log(foo); // ReferenceError
	let foo = "Foo";
	console.log(foo); // Foo
}
```
* accessible before declaration but undefined: `var`
_also known as "hoisting", because the var is "hoisted" to top of function scope, even though still undefined_
```javascript
function run() {
	console.log(foo); // undefined
	var foo = "Foo";
	console.log(foo); // Foo
}
```
