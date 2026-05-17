---
tags:
  - learning
  - programming
created: 2026-05-12
status: active
source:
topic: Rust Variables and Mutability
language: Rust
---

# Topic 
This is about the variables, basic types and how works this variables and who to use it.

>[!note]
>For default the variables are immutable, this offer [[rust]] to write code where we take advantage for concurrency.

When a variables is immutable, we can't change the value of this once a value is bound to a name  this mean the variable once a value is given this can't change. For define a variable in [[rust]] we can use de word `let`
### Example

```rust
fn main() {
	let x = 5;
	println!("The value of x is {}", x);
	x = 6;
	println!("The value of x is {}", x); 
}
```

In this example we have a error, when we try to compile, this response a error explain that we can not modification a variable immutable

```bash
$ cargo run
   Compiling variables v0.1.0 (file:///projects/variables)
error[E0384]: cannot assign twice to immutable variable `x`
 --> src/main.rs:4:5
  |
2 |     let x = 5;
  |         - first assignment to `x`
3 |     println!("The value of x is: {x}");
4 |     x = 6;
  |     ^^^^^ cannot assign twice to immutable variable
  |
help: consider making this binding mutable
  |
2 |     let mut x = 5;
  |         +++

For more information about this error, try `rustc --explain E0384`.
error: could not compile `variables` (bin "variables") due to 1 previous error
```

We can see that the same compiler explain how fix this error, for make a mutable variable we can add the world `mut`, this make a variable let it be mutable.

This error means that the compiler is saying the program is not safely doing what we want it to do.

### Mutable variables

How explain for can modify a variable we can add `mut` this make a variable can be mutable and this value can change.

### Example

```Rust
fn main() {
	let mut x = 5;
	println!("the value of x is {}", x);
	x = 6;
	println!("new value of x is {}", x);
}
```

In this case when we execute this program its running without problem
```bash
$ cargo run
   Compiling variables v0.1.0 (file:///projects/variables)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.30s
     Running `target/debug/variables`
The value of x is: 5
new value of x is: 6
```


## Idea principal

In this idea we have all variables immutables this is

---

## Simple Explanation (Feynman)
¿Cómo se lo explicarías a alguien sin conocimientos técnicos?

---

## Key Concepts

- 
- 
- 

---

## How works

## Step by Step 
1.
2.
3.

---

## Example practice

```example
```

---
## Mental Analogy 


---

## Problems that resolve
- 
- 

---

## Limitations 
* 
* 

---

## Real case use
- 
---

## Relationship of other topics

- [[ ]]

---

## Open Questions

---


