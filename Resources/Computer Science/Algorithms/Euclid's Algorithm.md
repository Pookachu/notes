`Finds the greatest common divisor between two numbers.`

Example code (Recursive)
```rust
fn gcd(a: u64, b: u64) -> u64 {
    if b == 0 { // Base case, can't modulus by 0
        a 
    } else {
        gcd(b, a%b) // Return b as new a, and a modulus b
    }
}
```