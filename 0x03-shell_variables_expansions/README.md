# 0x03. Shell, init files, variables and expansions

This project contains shell scripts that demonstrate mastery of shell variables, expansions, aliases, and arithmetic operations.

## Learning Objectives

- Understand shell initialization files (`/etc/profile`, `~/.bashrc`)
- Differentiate between local and global variables
- Work with environment variables and special parameters
- Perform shell expansions and command substitution
- Execute arithmetic operations in the shell
- Create and manage aliases

## Requirements

- All scripts tested on Ubuntu 20.04 LTS
- All scripts are exactly two lines long
- First line of all scripts: `#!/bin/bash`
- All scripts are executable
- No use of `&&`, `||`, or `;`
- No use of `bc`, `sed`, or `awk`

## Scripts

### Mandatory Tasks

| File | Description |
|------|-------------|
| `0-alias` | Creates an alias `ls` with value `rm *` |
| `1-hello_you` | Prints `hello user` where user is the current Linux user |
| `2-path` | Adds `/action` to the end of the PATH variable |
| `3-paths` | Counts the number of directories in the PATH |
| `4-global_variables` | Lists all environment variables |
| `5-local_variables` | Lists all local variables, environment variables, and functions |
| `6-create_local_variable` | Creates a local variable `BEST` with value `School` |
| `7-create_global_variable` | Creates a global variable `BEST` with value `School` |
| `8-true_knowledge` | Prints the result of 128 + the value in `TRUEKNOWLEDGE` variable |
| `9-divide_and_rule` | Prints the result of `POWER` divided by `DIVIDE` |
| `10-love_exponent_breath` | Displays the result of `BREATH` to the power of `LOVE` |
| `11-binary_to_decimal` | Converts a number from base 2 to base 10 |
| `12-combinations` | Prints all possible two-letter combinations except `oo` |
| `13-print_float` | Prints a number with two decimal places |

## Usage Examples

### Task 0: Creating an Alias
```bash
$ source ./0-alias
$ # The ls command is now aliased to rm * (be careful!)
```

### Task 1: Hello User
```bash
$ ./1-hello_you
hello julien
```

### Task 2: Add to PATH
```bash
$ echo $PATH
/usr/local/bin:/usr/bin:/bin
$ source ./2-path
$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/action
```

### Task 3: Count PATH Directories
```bash
$ ./3-paths
11
```

### Task 8: Arithmetic with Variable
```bash
$ export TRUEKNOWLEDGE=1209
$ ./8-true_knowledge
1337
```

### Task 11: Binary to Decimal
```bash
$ export BINARY=10100111001
$ ./11-binary_to_decimal
1337
```

### Task 12: Letter Combinations
```bash
$ ./12-combinations | wc -l
675
$ ./12-combinations | grep "oo"
$ # No output - oo is excluded
```

### Task 13: Float Formatting
```bash
$ export NUM=3.14159265359
$ ./13-print_float
3.14
```

## Repository

- **GitHub repository**: `alx-system_engineering-devops`
- **Directory**: `0x03-shell_variables_expansions`

## Author

ALX Software Engineering Program
