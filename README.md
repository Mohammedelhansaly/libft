# libft

## Introduction

The `libft` project is a foundational C library that reimplements standard C library functions and provides additional utility functions for C development. It is often used as a learning exercise to reinforce understanding of low-level programming, memory management, and modular code design. This library offers a reliable base for building more complex C projects by extending and customizing basic functionalities.

## Features

- Reimplementation of standard C library functions (`strlen`, `strcpy`, `memset`, etc.)
- Enhanced memory and string manipulation utilities
- List and array management functions
- Character checks and transformations
- Modular, well-documented C source code
- Custom data structures for improved flexibility

## Requirements

- GCC or Clang C compiler
- Make utility for build automation
- Compatible with Unix-like operating systems (Linux, macOS)
- Standard C library headers (e.g., `<string.h>`, `<stdlib.h>`)

## Installation

To use `libft` in your project, follow these simple steps:

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mohammedelhansaly/libft.git
   ```
2. **Navigate to the project directory**
   ```bash
   cd libft
   ```
3. **Build the library**
   ```bash
   make
   ```
   This will generate the `libft.a` static library file in the project root.

4. **Include the library in your project**
   - Add `libft.a` to your linker inputs.
   - Include the `libft.h` header in your source files.

## Usage

To use functions from `libft` in your C programs:

1. Include the header at the top of your source file:
   ```c
   #include "libft.h"
   ```

2. Link the static library when compiling:
   ```bash
   gcc your_program.c -L. -lft -o your_program
   ```

3. Example of using a `libft` function:
   ```c
   #include "libft.h"
   
   int main(void) {
       char str[50] = "Hello, world!";
       ft_strrev(str);
       printf("%s\n", str); // Output: "!dlrow ,olleH"
       return 0;
   }
   ```

## Configuration

`libft` typically does not require configuration for standard use. However, you can:

- **Add or remove source files**: Edit the `Makefile` to include or exclude specific modules as needed.
- **Custom macros and types**: Define custom macros or typedefs in `libft.h` for project-specific needs.
- **Compilation flags**: Modify `CFLAGS` in the `Makefile` for debug or optimization purposes.

## Contributing

Contributions are welcome to extend or improve `libft`. To contribute:

- Fork the repository and create your branch.
- Follow project coding style and naming conventions.
- Write descriptive commit messages.
- Add tests for new features or bug fixes.
- Submit a pull request with a summary of your changes.

**Contribution Process:**
1. Fork and clone the repository.
2. Create a new branch for your feature or fix.
3. Make and commit your changes.
4. Push to your fork.
5. Submit a pull request on GitHub.

---

For questions or support, please create an issue in the repository or contact the maintainer. Happy coding!
