# Abrupt

Abrupt is a comprehensive Rust library that provides a collection of cryptographic and mathematical utilities. It aims to offer efficient and easy-to-use implementations of common algorithms and functions.

## Core Functionalities

Abrupt provides a robust set of cryptographic and mathematical utilities:

### Cryptographic Operations
- Secure Hash Algorithms:
  - SHA-256
  - SHA-512
- Message Digest Algorithm:
  - MD5
- Data Encoding:
  - Base16 (Hexadecimal)
  - Base32
  - Base64

### Mathematical Utilities
- Array Computations:
  - Summation
  - Product calculation
  - Average determination
  - Minimum and maximum value extraction
- Number Theory:
  - Factorial computation
  - Greatest Common Divisor (GCD)
  - Least Common Multiple (LCM)
  - Primality testing
- Fundamental Mathematical Operations:
  - Exponentiation
  - Absolute value calculation
  - Value clamping

## Installation

Add this to your `Cargo.toml`:

```toml
[dependencies]
abrupt = "0.1.0"
```

## Usage

Here are some quick examples of how to use Abrupt:

```rust
use abrupt::crypto::{sha256, base64};
use abrupt::math::{factorial, is_prime};

fn main() {
    // Cryptography
    let hash = sha256(b"Hello, world!");
    println!("SHA-256 hash: {:?}", hash);

    let encoded = base64::encode(b"Abrupt is awesome!");
    println!("Base64 encoded: {}", encoded);

    // Mathematics
    let fact = factorial(5);
    println!("5! = {}", fact);


    let prime_check = is_prime(17);
    println!("Is 17 prime? {}", prime_check);
}
```

## License
Abrupt is released under the MIT License. See [LICENSE](LICENSE) for details.
