## `var` vs `let`
1. Scope
 * immediate function body: `var`
 * immediate enclosing block: `let`

2. Declaration
 * accessible before declaration but undefined: `var`
_also known as "hoisting", because the var is "hoisted" to top of function scope, but of course undefined until the value is set_
```javascript
function run() {
	console.log(foo); // undefined
	var foo = "Foo";
	console.log(foo); // Foo
}
```
 * not accessible until declaration: `let`
```javascript
function checkHoisting() {
	console.log(foo); // ReferenceError
	let foo = "Foo";
	console.log(foo); // Foo
}
```

3. Usage
 * Using `let` is critical in `for` loops... previously in Javascript if you declared a variable, say, `i`, with `var` in a `for` loop, this variable would persist after the completion of the `for` loop and anything that used `i` would use the final value of it, instead of the value at the time of the `for` loop execution 

Additional Resources:
1. https://2ality.com/2015/02/es6-scoping.html
2. https://exploringjs.com/es6/ch_variables.html
