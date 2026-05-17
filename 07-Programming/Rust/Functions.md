---
tags:
  - programming
language: Rust
framework:
created: 2026-05-16
---
# Topic 
The functions are very used in Rust. One of the principal functions used in the a lot programs is the function `main`, and to create a function we use a keyword `fn` that allow declare new functions.

>[!note]
>In rust all functions or variables use *snake case* the conventional style

```Rust
fn main() {
	println!("Hello world");
	
	another_function();
}

fn another_function() {
	println!("another function");
}
```

the functions execute in order that called in function main for this example first call `println` and after call `another_function`

### *Parameters*
we can define a function with parameters. when a function have parameters we need provide those concrete parameters 

```Rust
fn main() {
	another_function(5);
}

fn another_function(x: i32) {
	println("The value of x is {x}");
}
```

>[!note]
>We must declare the type of each parameter

### *Return values*
We have 2 forms to return of value in a function for this case we can describe that returned type value using `->` 
```Rust
fn sum(x: i32; y: i32) -> i32 {
	return {x + y};
}

fn main() {
	let result: i32 = sum(5, 4);
	
	println!("{result}");
}
```
This form to return value is explicit when we use keyword `return` and the end of expression use `;` semicolon
The other form to return is implicit in this case that must be returned don't use semicolon for example:
```Rust
fn square(x: i32) -> i32 {
	x * x
}

fn main() {
	let result = square(5);
	
	println!("Resulst square 5: {result}");
}
```

>[!Note]
For the case of implicit return is **not** compile if use semicolon to end of function 

---
## Important Concepts 

- We must declare type of parameters 
- We have 2 forms to return a value explicit and implicit 

---
##  Best Practices 
All functions use the `snake case` 
