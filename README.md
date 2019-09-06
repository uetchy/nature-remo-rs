# Nature Remo for Rust

[![Crates.io](https://img.shields.io/crates/v/remo)](https://crates.io/crates/remo)
[![Docs.rs](https://docs.rs/remo/badge.svg)](https://docs.rs/remo)
[![Travis (.com)](https://img.shields.io/travis/com/uetchy/nature-remo-rs)](https://travis-ci.com/uetchy/nature-remo-rs)

> Nature Remo API client for Rust.

**WARNING: This project is in heavily development state and not intended for production use.**

## Installation

```
cargo add remo
```

## Usage

```rust
extern crate remo;

use remo::cloud;

fn main() {
  let client = cloud::Client::new("<token>");
  let user = client.get_user()?
  println!("Name: {}", user.nickname)
}
```
