# Monkey Programming Language Interpreter

This project is an implementation of the Monkey programming language interpreter, following along with the book ["Writing an Interpreter in Go"](https://interpreterbook.com/) by Thorsten Ball.

## About Monkey Language

Monkey is a programming language designed specifically for learning interpreter and compiler implementation. It features:

- C-like syntax
- Variable bindings
- Integers and booleans
- Arithmetic expressions
- Built-in functions
- First-class and higher-order functions
- Closures
- A string data structure
- An array data structure
- A hash data structure

## Project Structure

The interpreter is implemented in Go and follows the book's structure:

- Lexer: Transforms source code into tokens
- Parser: Creates an Abstract Syntax Tree (AST) from tokens
- Evaluator: Executes the AST
- Object System: Represents values and their types

## Getting Started

### Prerequisites

- Go 1.11 or higher

### Building and Running

1. Clone the repository:
```bash
git clone https://github.com/yourusername/go-monkey.git
cd go-monkey
```

2. Build the project:
```bash
go build
```

3. Run the REPL:
```bash
./go-monkey
```

## Example Monkey Code

```monkey
// Binding a value to a name
let age = 1;

// Binding a function to a name
let add = fn(a, b) { return a + b; };

// Arrays
let myArray = [1, 2, 3, 4, 5];

// Hashes
let thorsten = {"name": "Thorsten", "age": 28};

// Higher order functions
let twice = fn(f, x) {
    return f(f(x));
};
```

## Learning Resources

- ["Writing an Interpreter in Go"](https://interpreterbook.com/) by Thorsten Ball
- [Official book repository](https://github.com/thorstenball/writing-an-interpreter-in-go)

## Acknowledgments

This implementation follows Thorsten Ball's excellent book "Writing an Interpreter in Go". The book provides a thorough, step-by-step guide to building an interpreter from scratch.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. This is an educational project following the book "Writing an Interpreter in Go" by Thorsten Ball. 