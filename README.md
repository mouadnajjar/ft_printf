
---

# ft_printf

`ft_printf` is a custom implementation of the `printf` function from the C standard library, designed to provide a basic understanding of how formatted output works in C. The project replicates the behavior of the `printf` function, supporting various format specifiers and providing a foundation for more advanced formatting options.

This project was developed as part of the [42 Network](https://www.intra.42.fr/) curriculum.

---

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)

---

## Description

`ft_printf` is a reimplementation of the `printf` function, which is part of the C standard library. The goal of this project was to implement this function from scratch, without using the standard library's `printf`, `sprintf`, or any other similar functions. 

The implementation focuses on understanding variadic functions, memory management, and the internal mechanisms of formatted output. It supports basic format specifiers and can handle different data types such as integers, strings, and characters.

---

## Features

`ft_printf` supports the following format specifiers:

- **%c** – Print a single character.
- **%s** – Print a string.
- **%p** – Print a pointer address in hexadecimal format.
- **%d / %i** – Print a signed integer.
- **%u** – Print an unsigned integer.
- **%x / %X** – Print an unsigned integer in hexadecimal format (lowercase/uppercase).
- **%f** – Print a floating-point number (if implemented in the future).

In addition to these basic specifiers, `ft_printf` handles flags, width, and precision.

---

## Installation

To use `ft_printf`, simply clone the repository to your local machine:

```bash
git clone https://github.com/mouadnajjar/ft_printf.git
cd ft_printf
```

Once you have the repository, you can compile it by including the provided `ft_printf.c` file in your project and linking it.

```bash
gcc -Wall -Werror -Wextra -o your_program your_program.c ft_printf.c
```

---

## Usage

To use `ft_printf`, include the `ft_printf.h` header file and call the `ft_printf` function in place of the standard `printf` function.

Example usage:

```c
#include "ft_printf.h"

int main() {
    ft_printf("Hello, %s!\n", "world");
    ft_printf("Number: %d\n", 42);
    ft_printf("Hex: %x\n", 255);
    return 0;
}
```

This will output:

```
Hello, world!
Number: 42
Hex: ff
```

---

## Examples

Here are some examples demonstrating the usage of various format specifiers:

```c
ft_printf("Character: %c\n", 'A');          // Output: Character: A
ft_printf("String: %s\n", "Hello, World!"); // Output: String: Hello, World!
ft_printf("Integer: %d\n", 1234);           // Output: Integer: 1234
ft_printf("Unsigned: %u\n", 1234);          // Output: Unsigned: 1234
ft_printf("Hexadecimal (lower): %x\n", 255); // Output: Hexadecimal (lower): ff
ft_printf("Hexadecimal (upper): %X\n", 255); // Output: Hexadecimal (upper): FF
ft_printf("Pointer: %p\n", (void *)0x1234);  // Output: Pointer: 0x1234
```

---

## Contributing

Contributions to this project are welcome! If you'd like to contribute, please fork the repository, make your changes, and create a pull request. Ensure that your code follows the project's coding style and passes any provided tests.



---
