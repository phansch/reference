# Never type

> **<sup>Syntax</sup>**\
> _NeverType_ : `!`

The never type `!` is a type with no values, representing the result of
computations that never complete. Expressions of type `!` can be coerced into
any other type.

```rust,should_panic
let x: ! = panic!();
// Can be coerced into any type.
let y: u32 = x;
```
