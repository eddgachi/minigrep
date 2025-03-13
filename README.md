# Minigrep

Minigrep is a simple command-line tool written in Rust that searches for a specified query within a given file.

## Features

- Reads a file and searches for a specific string.
- Displays the file content in the console.
- Handles errors gracefully.

## Prerequisites

- Install [Rust](https://www.rust-lang.org/tools/install) if you haven't already.

## Installation

Clone the repository and navigate to the project directory:

```sh
git clone <repository_url>
cd minigrep
```

Build the application:

```sh
cargo build --release
```

## Usage

Run the program with the following syntax:

```sh
cargo run -- <query> <filename>
```

Example:

```sh
cargo run -- rust main.rs
```

This will search for the word "rust" in the file `main.rs`.

Alternatively, if you have built the application:

```sh
./target/release/minigrep rust main.rs
```

## Error Handling

If incorrect arguments are provided, an error message is displayed:

```sh
Problem parsing arguments: not enough arguments
```

If the file is missing or cannot be read:

```sh
Application error: No such file or directory
```

## License

This project is open-source and available under the MIT License.
