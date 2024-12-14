# PooLang

A Tiny Interpreted but a Fast language written in Rust, featuring variable declarations, arithmetic operations, conditional statements, and control flow. This project includes a lexer, parser, and interpreter. The name `Poo` originates from Guinea Pig translated from `Burmese`.

## Crafted by **Shayy**

## 📜 Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Syntax Overview](#syntax-overview)
- [Example Code](#example-code)
- [Development](#development)
- [Contributing](#contributing)

## ✨ Features

- **Arithmetic Expressions**: Supports addition, subtraction, multiplication, and division with correct operator precedence.
- **Variable Declarations**: Uses `poo` keyword for variable declarations.
- **Mutable Variables**: Like in Rust, all variables are immutable by default. Uses `mut` instead of `poo` for mutable variables.
- **Conditional Statements**: Includes `if`, and `else` for branching.
- **Control Flow**: Supports `while` and `for in` loops and `return` statements.
- **Custom Operators**:
  - Short hand syntax for assignment: `<:`
  - Assignment and Reassignment operator: `=`
  - Arrow operator: `>>`
- **Lexer, Parser, and Interpreter**: A full pipeline from tokenizing source code to executing it.

## 🚀 Installation

1. Curl the latest release.

```bash
curl -L https://github.com/shayyz-code/poo/releases/download/v0.1/poo > poo
```

2. Consider the installation directory.

```bash
cd ~/Downloads && mkdir ~/poo && mv ./poo ~/poo
```

3. Add it to your Environment Variables.

```bash
export PATH=~/poo:$PATH
```

## 🛠️ Usage

To run the interpreter on a source file:

```bash
poo <path_to_your_source_file>
```

Example:

```bash
poo app.poo
```

## 📝 Syntax Overview

The language features basic syntax for arithmetic, variable declarations, and control flow:

### **Variable Declarations**

Both in short hand and regular assignment operator.

```poo
poo x <: 10;
mut y int = 5 + 2 * 3;
```

### **Arithmetic Operations**

```poo
poo result int = x + y * 2 - 10 / 2;
```

### **Conditional Statements**

```poo
if x > y {
    return x;
} else {
    return y;
}
```

### **Loops**

```poo
use std::pout;

mut count <: 0;

while count < 10 {
    count = count + 1;
}

for i in 0..4 step 2 {
    pout("Hello, World ", i);
}
```

### **Functions**

```poo
use std::pout;

poof getName () >> string {
    poo name <: "Shayy";
    return name;
}

pout(getName());
```

## 📚 Example Code

Example codes are provided in this repo.
Try a rotating donut in my PooLang :D

```bash
git clone https://github.com/shayyz-code/poo

```

```bash
cd ./poo

```

```bash
./poo examples/donut.poo

```

## Test the speed

```bash
poo examples/app.poo --speed
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue if you find a bug or have a feature request.

### Steps to Contribute

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your feature description"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a Pull Request.

## 💬 Feedback

If you have any questions or feedback, feel free to reach out or open an issue in the repository.

---

Happy Coding! 🎉

---
