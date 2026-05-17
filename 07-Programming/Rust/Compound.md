---
tags:
  - learning
  - programming
created: 2026-05-16
---
# Idea
This means a group of multiples values into in one type. [[Rust]] have 2 primitives types which are `tuples` and `arrays`

## Concept

### Tuples
A tuple is used to store a diferents types of values into a one compound type. 
> [!Note]
> The tuples have a fixed length: One declared this can not grow or shrink in size

For create a tuple we can use comma-separated list of values inside of parentheses. for example
```Rust
let tup: (i32, f64, u8) = (-500, 6.4, 8);
```

For get a individuals values of tuples we can do this:
```Rust
fn main() {
	let tup = (-500, 6.4, 1);	
	
	let (x, y, z) = tup;
	
	println!("The value of y is {y}");
}
```

this form is for get values is called *destructuring* because its breaks the single tuple into three parts.
We can access too directly by using a period `.` 
```Rust
fn main() {
	let x = (-500, 6.4, 1);	
	
	let five_hundred = x.0;
	let six_point_four = x.1; 
	let one = x.2;
	
	println!("three value of tuple is {one}");
}
```
### Arrays

Array is another collection of multiple values same type. In [[Rust]] have a fixed length

```Rust
fn main() {
	let a = [1, 2, 3, 4, 5];
}
```

we can write the array using square brackets with the type of each element, semicolon, and number of elements in the array.
```Rust
fn main() {
	let a: [i32; 5] = [1, 2, 3, 4, 5];
}
```

---
## Relationship 

- [[Data Types]]
