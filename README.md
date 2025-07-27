# Monkey Programming Language

A simple programming language interpreter written in Go, featuring a lexer, parser, AST, and tree-walking evaluator.

## Features

- **Lexical Analysis**: Tokenizes Monkey source code
- **Parsing**: Builds an Abstract Syntax Tree (AST) from tokens
- **Evaluation**: Tree-walking interpreter with environment support
- **REPL**: Interactive Read-Eval-Print Loop
- **Built-in Functions**: Core functionality for the language

## Project Structure

```
monkey/
├── ast/           # Abstract Syntax Tree definitions
├── evaluator/     # Tree-walking interpreter and built-ins
├── lexer/         # Lexical analyzer (tokenizer)
├── object/        # Object system and environment
├── parser/        # Parser with tracing support
├── repl/          # Read-Eval-Print Loop
├── token/         # Token definitions
└── main.go        # Entry point
```

## Usage

Run the REPL:

```bash
go run main.go
```

## Testing

Run tests for all packages:

```bash
go test ./...
```

Run tests for a specific package:

```bash
go test ./lexer
go test ./parser
go test ./evaluator
```

## Development

This interpreter implements the Monkey language as described in "Writing an Interpreter in Go" by Thorsten Ball.