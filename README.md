
# ft_printf

## Overview
`ft_printf` is a custom implementation of the C standard library function `printf`. It aims to mimic the behavior of `printf`, allowing for formatted output to the standard output. This function is often a part of systems programming and school projects where students reimplement standard C library functions.

## Features
- Handles various format specifiers like `%d`, `%s`, `%c`, `%x`, and more.
- Supports width, precision, and flag modifiers.
- Capable of printing to standard output with formatting.

## Usage

### Function Prototype
```c
int ft_printf(const char *format, ...);
```

### Parameters
- `format`: A string that contains the text to be written to stdout. It can optionally contain embedded format specifiers that are replaced by the values specified in subsequent additional arguments.

### Return Value
- The number of characters printed (excluding the null byte used to end output to strings)

## Example
```c
#include "ft_printf.h"

int main(void)
{
    ft_printf("Hello, %s!", "world");
    return (0);
}
```
This example will print `Hello, world!` to the standard output.

## Installation and Compilation
Include the `ft_printf` source and header files in your project directory. Compile them along with your project files.

```bash
gcc -Wall -Wextra -Werror main.c ft_printf.c -o myprogram
```

## Customization
You can extend `ft_printf` by adding more format specifiers or features according to your project requirements.
