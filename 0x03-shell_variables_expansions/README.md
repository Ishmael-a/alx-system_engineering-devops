# 0x03. Shell, init files, variables and expansions

This project contains shell scripts that demonstrate the use of shell variables, expansions, aliases, and arithmetic operations in Bash.

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All scripts tested on Ubuntu 20.04 LTS
- All scripts are exactly two lines long
- All files end with a new line
- First line of all files: `#!/bin/bash`
- Not allowed to use: `&&`, `||`, `;`, `bc`, `sed`, or `awk`
- All files must be executable

## Files Description

### Mandatory Tasks

| File | Description |
|------|-------------|
| `0-alias` | Creates an alias `ls` with value `rm *` |
| `1-hello_you` | Prints "hello user" where user is the current Linux user |
| `2-path` | Adds `/action` to the end of the PATH variable |
| `3-paths` | Counts the number of directories in the PATH |
| `4-global_variables` | Lists all environment variables |
| `5-local_variables` | Lists all local variables, environment variables, and functions |
| `6-create_local_variable` | Creates a local variable `BEST` with value `School` |
| `7-create_global_variable` | Creates a global variable `BEST` with value `School` |
| `8-true_knowledge` | Prints the result of adding 128 to the value in `TRUEKNOWLEDGE` |
| `9-divide_and_rule` | Prints the result of `POWER` divided by `DIVIDE` |
| `10-love_exponent_breath` | Displays the result of `BREATH` to the power of `LOVE` |
| `11-binary_to_decimal` | Converts a number from base 2 to base 10 (stored in `BINARY`) |
| `12-combinations` | Prints all possible combinations of two letters (except `oo`) |
| `13-print_float` | Prints a number with two decimal places (stored in `NUM`) |

### Advanced Tasks

| File | Description |
|------|-------------|
| `100-decimal_to_hexadecimal` | Converts a number from base 10 to base 16 (stored in `DECIMAL`) |
| `101-rot13` | Encodes and decodes text using ROT13 encryption |
| `102-odd` | Prints every other line from input, starting with the first line |
| `103-water_and_stir` | Adds two numbers in custom bases and prints result in base `bestchol` |

## Usage Examples

### Basic Examples

```bash
# 0-alias
$ source ./0-alias
$ ls  # This will execute rm *

# 1-hello_you
$ ./1-hello_you
hello julien

# 2-path
$ source ./2-path
$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/action

# 8-true_knowledge
$ export TRUEKNOWLEDGE=1209
$ ./8-true_knowledge
1337
```

### Advanced Examples

```bash
# 100-decimal_to_hexadecimal
$ export DECIMAL=16
$ ./100-decimal_to_hexadecimal
10

# 101-rot13
$ echo "Hello World" | ./101-rot13
Uryyb Jbeyq

# 102-odd
$ ls -1 | ./102-odd
# Prints every other line
```

## Installation

Clone the repository:
```bash
git clone https://github.com/yourusername/alx-system_engineering-devops.git
cd alx-system_engineering-devops/0x03-shell_variables_expansions
```

Make all scripts executable:
```bash
chmod +x *
```

## Author

ALX System Engineering & DevOps Project

## Learning Objectives

By completing this project, you should be able to:
- Explain what happens when you type `$ ls -l *.txt`
- Understand shell initialization files (`/etc/profile`, `/etc/inputrc`, `~/.bashrc`)
- Differentiate between local and global variables
- Work with shell expansions and arithmetic operations
- Create and use aliases
- Perform arithmetic operations in shell scripts
- Convert between different number bases

## Resources

- [Expansions](http://linuxcommand.org/lc3_lts0080.php)
- [Shell Arithmetic](https://www.gnu.org/software/bash/manual/html_node/Shell-Arithmetic.html)
- [Shell Variables](https://www.gnu.org/software/bash/manual/html_node/Shell-Parameters.html)
- [Shell Initialization Files](http://www.gnu.org/software/bash/manual/html_node/Bash-Startup-Files.html)