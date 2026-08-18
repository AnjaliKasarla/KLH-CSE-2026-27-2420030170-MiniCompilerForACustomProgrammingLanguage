# Mini Compiler for a Custom Programming Language

A Compiler Design project that implements the major phases of a compiler for a simple custom programming language. The project demonstrates how high-level source code is transformed into optimized target code through lexical analysis, parsing, intermediate code generation, optimization, and code generation.

---

## Project Details

| Field | Details |
|---|---|
| **Project Title** | Mini Compiler for a Custom Programming Language |
| **Course** | Project Evaluation (24CS2235E) |
| **Academic Year** | 2026–2027 |
| **Guide** | P. Krishna Kishore |

---

## Team Members

| S. No. | University ID | Name |
|---:|---:|---|
| 1 | 2420030170 | Anjali Kasarla |
| 2 | 2420030212 | Vinusha Muppala |
| 3 | 2420030743 | M Lakshmi Abhista |

---

## Abstract

The **Mini Compiler for a Custom Programming Language** is a Compiler Design project that implements the major phases of a compiler for a simple, user-defined programming language. The system accepts source code written in the custom language and translates it into optimized target code through a sequence of compilation phases.

The project begins with **lexical analysis**, where the source program is converted into tokens using **regular expressions and finite automata (DFA)**. These tokens are then processed by a **parser** based on a context-free grammar to validate the syntactic structure of the program and construct an **Abstract Syntax Tree (AST)**. The AST is used as an intermediate representation for generating **Three Address Code (TAC)**.

The generated intermediate code is optimized using techniques such as **constant folding, constant propagation, common subexpression elimination, and dead code elimination**. Finally, the optimized intermediate code is translated into simple **target/machine-like code** through code generation.

The project provides practical implementation of important Compiler Design concepts including lexical analysis, regular expressions, finite automata, parsing, syntax-directed translation, abstract syntax trees, intermediate code generation, code optimization, and target code generation.

---

## Objectives

- To understand and implement the major phases of a compiler.
- To design a simple custom programming language with a well-defined syntax.
- To implement lexical analysis using regular expressions and finite automata.
- To develop a parser for validating the syntax of source programs.
- To construct an Abstract Syntax Tree (AST).
- To generate Three Address Code (TAC) as an intermediate representation.
- To implement basic code optimization techniques.
- To generate simple target/machine-like code from optimized intermediate code.
- To demonstrate the complete transformation from high-level source code to low-level target code.

---

## Compiler Architecture

```text
                 Source Program
                       |
                       v
              +------------------+
              | Lexical Analyzer |
              +------------------+
                       |
                       v
                    Tokens
                       |
                       v
              +------------------+
              |     Parser       |
              +------------------+
                       |
                       v
              Parse Tree / AST
                       |
                       v
              +------------------+
              | Syntax Directed  |
              |   Translation    |
              +------------------+
                       |
                       v
             Three Address Code
                       |
                       v
              +------------------+
              | Code Optimizer   |
              +------------------+
                       |
                       v
              Optimized 3AC
                       |
                       v
              +------------------+
              | Code Generator   |
              +------------------+
                       |
                       v
                 Target Code
