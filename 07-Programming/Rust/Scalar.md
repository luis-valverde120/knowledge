---
tags:
  - learning
created: 2026-05-16
---
# Idea
the scalar type represent a single values like *bolean, number, float* or *char* 
We have values how:
- Integer 1, 2, 3, 4
- Float 1.1, 1.2, 1.3
- Bolean `true` or `false`
- Character  `a`, `b`, `c`
## Concept
#### *Integers*
An integer is a number without faction part, for example 1, 2 or 100
In integers number we have two types `signed integers` or `unsigned integers`.

##### Signed Integers
This means the integers that have a values positives o negatives like 1 or -1 we can be stored from $-2^{n-1}$ to $2^{n-1}$ for example if we use a 16bits we can store from -32768 to 32768

this represented using the letter `i`
```Rust
let x: i32 = 20;
let y: i32 = -10;
```

##### Unsigned Integers
This means the integers we can use only positive numbers. in this type we don't have a number negatives. for example for `i8` we hava to store from **0 to 128**.

| **Length** | **Signed** | **Unsigned** |
| ---------- | ---------- | ------------ |
| 8-bits     | `i8`       | `u8`         |
| 16-bits    | `i16`      | `u16`        |
| 32-bits    | `i32`      | `u32`        |
| 64-bits    | `i64`      | `u64`        |
| 128-bits   | `i128`     | `u128`       |
| arch       | `isize`    | `usize`      |
>[!note]
>for `isize` and `usize` this depend of architecture this mean this integer adapts to the different architectures of processor.

#### *Floating-Point*
In [[rust]] we have two types of floating-point numbers for handle decimals. The two types are `f32`and `f64` for default [[rust]] use of 64 bits because is the most modern in CPUs 

```Rust
let x = 2.5; // this use f64
let y: f32 = 2.3334; // this use f32
```

#### *Boolean*
This are values `true` or `false`
```rust
let is_true = true;
let is_false: bool = false;
```

#### *Char*
This is a values like 'a' or 'b'
```rust
let c = 'c';
let l: char = 'l'
```

---

## Expanation 
This is primitives values we can use to make sums o save names etc.

---

## Relationship 
- [[Data Types]]

