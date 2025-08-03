# ALX System Engineering & DevOps - Shell Variables and Expansions

This repository contains solutions to the ALX School project on shell variables and expansions. The project focuses on understanding and implementing various shell scripting concepts including variables, expansions, and shell arithmetic.

## Project Overview

This project is part of the ALX Software Engineering program's System Engineering & DevOps track. It covers fundamental concepts of shell scripting with emphasis on:

- Shell variables (local and global)
- Environment variables
- Variable expansions
- Shell arithmetic
- Command substitution
- Special parameters

## Learning Objectives

By the end of this project, you should be able to explain:

- What happens when you type `$ ls -l *.txt`
- What are the `/etc/passwd` and `/etc/shadow` files
- What is the difference between a local and global variable
- What is a reserved variable
- How to create, update and delete shell variables
- What are the roles of special parameters
- What are expansions and how to use them
- What is the difference between single and double quotes
- How to do command substitution with `$()` and backticks

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All scripts tested on Ubuntu 20.04 LTS
- All scripts should be exactly two lines long (`wc -l file` should print 2)
- All files should end with a new line
- The first line of all files should be exactly `#!/bin/bash`
- All files must be executable

## Files Description

| File | Description |
|------|-------------|
| `1-hello_you` | Script that prints "hello" followed by the current Linux user |
| `2-path` | Script that adds `/action` to the PATH |
| `3-paths` | Script that counts the number of directories in the PATH |
| `4-global_variables` | Script that lists environment variables |
| `5-local_variables` | Script that lists all local variables and environment variables, and functions |
| `6-create_local_variable` | Script that creates a new local variable |
| `7-create_global_variable` | Script that creates a new global variable |
| `8-true_knowledge` | Script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE |
| `9-divide_and_rule` | Script that prints the result of POWER divided by DIVIDE |
| `10-love_exponent_breath` | Script that displays the result of BREATH to the power LOVE |
| `11-binary_to_decimal` | Script that converts a number from base 2 to base 10 |
| `12-combinations` | Script that prints all possible combinations of two letters, except `oo` |
| `13-print_float` | Script that prints a number with two decimal places |

## Usage

To run any of the scripts, make sure they are executable:

```bash
chmod +x script_name
./script_name
```

### Examples

**Hello User:**

```bash
$ ./1-hello_you
hello guillaume
```

**Add to PATH:**

```bash
$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
$ source ./2-path
$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/action
```

**Binary to Decimal:**

```bash
$ export BINARY=10100111001
$ ./11-binary_to_decimal
1337
```

**Combinations:**

```bash
$ ./12-combinations | head -10
aa
ab
ac
ad
ae
af
ag
ah
ai
aj
```

## Project Structure

```text
alx-system_engineering-devops/
├── README.md
├── 1-hello_you
├── 2-path
├── 3-paths
├── 4-global_variables
├── 5-local_variables
├── 6-create_local_variable
├── 7-create_global_variable
├── 8-true_knowledge
├── 9-divide_and_rule
├── 10-love_exponent_breath
├── 11-binary_to_decimal
├── 12-combinations
├── 13-print_float
└── 0x03-shell_variables_expansions/
```

## Key Concepts Covered

### Variables

- **Local Variables**: Variables that exist only within the shell session where they were created
- **Global Variables**: Environment variables that are available to child processes
- **Special Parameters**: `$0`, `$1`, `$2`, etc., `$#`, `$@`, `$*`, `$$`, `$?`

### Expansions

- **Parameter Expansion**: `${parameter}`
- **Command Substitution**: `$(command)` or `` `command` ``
- **Arithmetic Expansion**: `$((expression))`
- **Brace Expansion**: `{a..z}`, `{1..10}`

### Arithmetic Operations

- Addition: `$((a + b))`
- Subtraction: `$((a - b))`
- Multiplication: `$((a * b))`
- Division: `$((a / b))`
- Exponentiation: `$((a ** b))`
- Base conversion: `$((base#number))`

## Author

### Derick Obeng

- ALX Student
- System Engineering & DevOps Track

## Acknowledgments

- ALX School for providing the project requirements and learning framework
- The Bash manual for comprehensive documentation on shell features

## License

This project is part of the ALX curriculum and is intended for educational purposes.

---

*This project is part of the ALX Software Engineering Program's System Engineering & DevOps track.*
