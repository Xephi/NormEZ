# NormEZ

Coding-style checker for Epitech students. This program analyzes your C source files for Epitech coding-style violations.

*FR:* Moulinette de norme pour les étudiants d'Epitech. Cette norminette cherche des erreurs de norme Epitech dans vos fichers de code source C.

## Requirements

 - [Ruby](https://www.ruby-lang.org/en/)

### Installing Ruby on Fedora (Epitech's dump 2017)

```
sudo dnf install ruby
```

## How to use NormEZ?

 - Clone the repository:
```
git clone https://github.com/ronanboiteau/NormEZ
```
 - Copy the `NormEZ.rb` executable in your project repository.
 - Run NormEZ:
```
ruby NormEZ.rb
```
 - NormEZ will recursively search for `.c` and `.h` files to analyze in your current directory.

## Features

Here are the Epitech coding-style violations checked by NormEZ:
 - Lines with too many columns (> 80).
 - Forbidden files: every regular file that does not match `Makefile`, `*.c` or `*.h` (ex: `*.o`, `*.gch`, `bsq`, ...).
 - *[Not exhaustive]* Too broad filenames (ex: `string.c`, `algo.c`, `my_algorithm.c`, ...).
 - Missing or corrupted header.
 - Functions that contain more than 20 lines.
 - Several semicolon-separated assignments on the same line.
 - Forbidden keyword (`goto`).
 - *[Not exhaustive]* Forbidden function (`printf()`, `dprintf()`, `atoi()`, `memcpy()`, `scanf()`, `strlen()`, `strdup()`, ...).
 - Too many `else if` statements.
 - Trailing space(s) and/or tabulation(s) at the end of a line.
 - Space(s) in indentation.
 - Too many functions in file (> 5).
 - Functions with no parameters that don't take void as argument in their declaration.
 - Functions with too many arguments (> 4).
 - Missing space after keyword.
 - Misplaced pointer symbol(s).
 - Filenames that don't respect the [snake_case naming convention](https://en.wikipedia.org/wiki/Snake_case).

## To-do

Here are the Epitech coding-style violations ***NOT YET*** checked by NormEZ:
 - Wrong indentation level.
 - Folder names that don't respect the [snake_case naming convention](https://en.wikipedia.org/wiki/Snake_case).

## Bugs

### Known bugs

 - `for` statements been flagged as multiple assignments.

### Report a bug

If you found a bug that isn't listed above in as a known bug, feel free to [create a GitHub issue](https://github.com/ronanboiteau/NormEZ/issues).

## Author

* **Ronan Boiteau** ([GitHub](https://github.com/ronanboiteau) / [LinkedIn](https://www.linkedin.com/in/ronanboiteau/))
