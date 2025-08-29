# wiffles
Testing rust library

# Using

1. Start a new cargo project with `cargo new import_wiffles`
2. Edit Cargo.toml, and add dependency:

```
[package]
name = "import_wiffles"
version = "0.1.0"
edition = "2021"

[dependencies]
wiffles = { git = "https://github.com/richardforth/wiffles", branch = "main" }
```

3. Edit `src/main.rs` in your project

```
fn main() {
    let my_string = String::from("Import successful!");
     wiffles::say(my_string);
}

```

# Cargo Build
```
$ cargo build
    Updating git repository `https://github.com/richardforth/wiffles`
     Locking 1 package to latest compatible version
   Compiling wiffles v0.0.3 (https://github.com/richardforth/wiffles?branch=main#b072fbd3)
   Compiling import_wiffles v0.1.0 (/home/rforth/git/rust/playground/import_wiffles)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 1.07s
17:37:22 $ cargo run
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/import_wiffles`
Wiffles says: 'Import successful!'
$ 

```

## Thats all it does at the moment, this was an experiment on hosting rust libraries on GitHub
