---
tags:
  - programming
language: Rust
framework:
created: 2026-05-16
---
# Topic 
This is a basic of programming, this is the ability of run a some section of code if this condition is `true` or run some code repeatedly when the condition is `true`. 
The common structures of control flow is `if` expressions and loops

## Important Concepts 

- ### *if condition* 
this allow execute a branch of code depend of the condition, for example if we need evaluate a person is of legal age we must be use a `if` evaluating the age of person if this person has more than 18 this is a legal person in other case this is a minor. for example

```Rust
fn main() {
	let age_bob: i32 = 19;
	
	if age_bob >= 18 {
		println!("Bob is a legal age {age_bob}");
	} else {
		println!("Bob is minor");
	}
}
```

- #### *Multiple condition using else if*
in this case we can evaluate a different values of a condition, for example a students that has 3 cases *reproved*, *approved*, *supplementary exam* if the student have an average greater than 7 this is approved, if the student have a average greater than 5 and less than 7 this is supplementary exam and otherwise the student reprove 

```Rust
fn main() {
	let average = 6.2;
	
	if average >= 7 {
		println!("The student approved with grade {average}");
	} else if average >= 5 && average < 7 {
		println!("The student supplementary exam with grade {average}");
	} else {
		println!("The student reprove with grade {average}");
	}
}
```

- #### *If in assignments*
we can assign a value of returned of condition in a variable this based in conditions
```Rust
fn main() {
	let is_even = if number % 2 == 0 { true } else { false };
	println!("is the number even? {}", is_even);
}
```

- ### *Loops*
this are block of code than execute more than once. in [[rust]] we have different types of loops `for`, `loop`, `while`.

- #### *Code with loop* 
the keyword loop execute a infinite block of code, this continue until explicitly interrupted using `break`
```Rust
fn main(){
	let mut count = 0;
	
	loop {
		println!("Count {}", count);
		count += 1;
		
		if count == 5 {
			break;
		}
	}
}
```

We can use loop to return a value out

```Rust
fn main() {
	let mut counter = 0;
	
	let result = loop {
		counter += 1;
		
		if counter == 10 {
			break counter * 22 2
		}
	}
	
	println!("The result of counter: {}", result);
}
```

We can declare a `loop` inside `loop` To void loops problem in [[rust]] we have a **loop labels**. This allow we can use the `break` or `continue` statements in a specific `loop`

```Rust
'outer loop {
	'inner loop {
		if some_condition {
			break 'inner;
		}
		
		if another_condition {
			break 'outer;
		}
	}
}
```

- #### *While*
While execute a block of code when the condition is `true`
```Rust
fn main() {
	let mut number = 1;
	
	while number  <= 5 {
		println!("Number is {}", number);
		number += 1;
	}
}
```

- #### *For*
for is use to iterate a range or iterate a collection, on an iterable object 
```Rust
fn main() {
	for number in (1...=3).rev() {
		println!("{number}");
	}
}
```

Example when iterable object 
```Rust
fn main {
	let numbers = [1, 2, 3, 4, 5, 6, 7, 8];
	for number in numbers.iter() {
		println!("Number: {}", number)
	}
}
```
the `.iter()` is to create a object iterable from array of numbers. this method not consume the array, its only borrow the elements of array.
```Rust
fn main {
	let numbers = [1, 2, 3, 4, 5, 6];
	for number in numbers {
		println!("Number: {number}");
	}
}
```
