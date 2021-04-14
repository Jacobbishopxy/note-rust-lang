# Note Rust Lang

A study note of Rust language.

Official references:

- [The Rust Programming Language](https://doc.rust-lang.org/book)
- [Rust by Example](https://doc.rust-lang.org/rust-by-example/index.html)
- [Rustlings](https://github.com/rust-lang/rustlings)
- [The Cargo Book](https://doc.rust-lang.org/cargo/index.html)
- [The Rustonomicon](https://doc.rust-lang.org/nomicon/): Unsafe Rust Programing

Other useful references:

- [pretzelhammer/rust-blog](https://github.com/pretzelhammer/rust-blog)
- [rust-unofficial/too-many-lists](https://rust-unofficial.github.io/too-many-lists/index.html)
- [rust-unofficial/patterns](https://rust-unofficial.github.io/patterns/)
- [Possible Rust](https://www.possiblerust.com/)

## Project Structure

```null
├── doc
│   ├── Rust By Example
│   └── The Rust Programming Language
│
├── trpl
│   ├── Cargo.toml
│   ├── src
│   │   ├── minigrep
│   │   │   ├── data.rs
│   │   │   └── func.rs
│   │   ├── blog.rs
│   │   ├── gui.rs
│   │   ├── hello_macro.rs
│   │   ├── lib.rs
│   │   ├── messenger.rs
│   │   ├── minigrep.rs
│   │   └── oop_encapsulation.rs
│   └── trpl_derive
│       ├── src
│       │   └── lib.rs
│       └── Cargo.toml
│
├── trpl_example
│   ├── Cargo.toml
│   └── src
│       ├── bin
│       │   ├── blog.rs
│       │   ├── gui.rs
│       │   ├── hello_macro.rs
│       │   └── minigrep.rs
│       └── main.rs
│
├── Cargo.lock
├── Cargo.toml
├── README.md
└── target
```

### trpl [lib]

- minigrep: book TRPL chapter 12
- messenger: book TRPL chapter 15.5
- oop_encapsulation: book TRPL chapter 17.1
- gui: book TRPL chapter 17.2
- blog: book TRPL chapter 17.3
- hello_macro: book TRPL chapter 19.5

### trpl_example [bin]

- blog run:
  `cargo run -p trpl_example --bin blog`

- minigrep run:
  `cargo run -p trpl_example --bin minigrep -- the poem.txt`
  or
  `CASE_INSENSITIVE=1 cargo run -p trpl_example --bin minigrep -- the poem.txt`

- minigrep test:
  `cargo test -p trpl -- tests_minigrep`

- gui run:
  `cargo run -p trpl_example --bin gui`

- hello_macro run:
  `cargo run -p trpl_example --bin hello_macro`
