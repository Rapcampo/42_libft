# Table of contents
- [Overview](#overview)
    + [written in C and accordance with the norm](#written-in-c-and-accordance-with-the-norm)
  * [Mandatory part](#mandatory-part)
  * [Technical considerations](#technical-considerations)
  * [Functions to be included](#functions-to-be-included)
- [Function Breakdown](#function-breakdown)
  * [Mandatory Functions](#mandatory-functions)
    + [<ctype.h> Functions](#ctypeh-functions)
    + [<string.h> Functions](#stringh-functions)
    + [<stdlib.h> Functions](#stdlibh-functions)
    + [Non-Standard Functions](#non-standard-functions)
  * [Bonus Functions](#bonus-functions)
- [The Norm](#the-norm)

# Overview

This is the first project of the common core for the 42 programming school, as such it follow  general guidelines that must be complient with the school ☠️[norm](#the-norm)☠️ for readability of the code. The following are the general rules for this project.

### written in C and accordance with the norm 
- Must be completely error free, no seg fault, bus error, double free... undefined is ok, if it happens once. 
- No memory leaks! always free heap memory properly!  
- Must submit a makefile if required, the make file must compile with the usual flags -Werror, -Wextra, -Wall, Makefile must not relink.  
- Must contain the rules $(name), all, clean, fclean and re.  
- If bonuses are wanted, must include a rule in the makefile.  
- Bonuses must be in a different file "_bonus.c or _bonus.h"  if your project allows you to use your libft folder with its makefile. your project makefile must compile the library by using its makefile then the project.
- It is encouraged to create your own test programs.  

## Mandatory part
 
 - Files: Makefile, libft.h, ft_*.c 
 - Makefile: NAME, all, clean, fclean, re.
 - External functions: Malloc, Free, Write (Depeding on the project).
 - Write your own library: a collection of useful functions that will be a useful tool for your cursus;  
   
## Technical considerations  
 
- Declaring global variables is forbidden.  
- If you need helper functions to split a more complex function, they must be defined as **static**. so their scope becomes limited to the appropriate file. 
- Place all the files at the root of the repository.  
- Unused files are forbidden.  
- Every .c file must be compiled with the flags -Wall -Wextra -Werror.  
- Must use the command ar to create your library. using libtool is forbidden.  
- Your libft.a has to be created at the root of your repository.  
   
## Functions to be included
- Redo a set of libc functions. same prototype, same behaviours. only difference must be their names.  
- They must use the ft_ prefix.

# Function Breakdown

For each function there will be a brief description with a link to a detailed wiki style overview of how the function works (work in progress...). This detailed description is done with the porpuse of a better understanding of how each of these function works as well as the structure of their syntax. 

## Mandatory Functions

### <ctype.h> Functions

| Function Name| Description | Status |
|--------|--------|:--------:|
 |ft_isalpha | Checks for an alphabetic character, either lowercase or uppercase. | ✔️ |
 |ft_isdigit | Checks for a digit between 0 through 9. | ✔️ |
 | ft_isalnum | Checks if the character is alphanumeric. | ✔️ |
| ft_isascii | Checks if the character is part of the ASCII table. | ✔️ |
| ft_isprint | Checks whether a character is printable. | ✔️ |
| ft_toupper | Coverts a character to uppercase. | ✔️ |
| ft_tolower | Converts a character to lowercase. | ✔️ |

### <string.h> Functions

| Function Name| Description | Status |
|--------|--------|:--------:|
| ft_memset | Fill memory with a constant byte. | ✔️ |
| ft_strlen | Takes a string and return its length. | ✔️ |
| ft_bzero | Erases the data in the ___n___ byes of the memory. | ✔️ | 
| ft_memcpy | Copy memory area. (does not support overlap) | ✔️ |
| ft_memmove | Copy memory area. (supports overlapping) | ✔️ |
| ft_strlcpy | Size bound string copying. | ✔️ |
| ft_strlcat | Size bound string concatenation. | ✔️|
| ft_strchr | Locate the first occurance of a character in a given string. | ✔️ |
| ft_strchrr | Locate the last occurance of a character in a given string. | ✔️ |
| ft_strncmp | Compare two strings, in a given ___N___ size. | ✔️ |
| ft_memchr | Locate a character in memory area. | ✔️ |
| ft_memcmp | Compare memory areas. | ✔️ |
| ft_strnstr | Locates a substring in a given string | ✔️ |
| ft_strdup | Creates a duplicate of the input string | ✔️ |

### <stdlib.h> Functions

| Function Name| Description | Status |
|--------|--------|:--------:|
| ft_atoi | Converts a string into an integer. | ✔️ |
| ft_calloc | Allocates a memory area and sets its bytes' values to 0 | ✔️ |

### Non-Standard Functions

| Function Name| Description | Status |
|--------|--------|:--------:|
| ft_substr | Returns a substring from a string | ✔️ |
| ft_strjoin | Concatenates two strings. | ✔️ |
| ft_strtrim | Trims the beginning and end of a string with a specific set of characters. | ✔️ |
| ft_split | Split a string into smaller strings using a character as delimiter. | ✔️ |
| ft_itoa | Converts integer numbers into a string. | ✔️ |
| ft_strmapi | Copies a string and applies a function to each character of the new allocated copy string | ✔️ |
| ft_striteri | Applies a given function to each character of a string. | ✔️ |
| ft_putchar_fd | Outputs a char into a file descriptor. | ✔️ |
| ft_putstr_fd | Outputs a string into a file descriptor. | ✔️ |
| ft_putendl_fd | Outputs a string into a file descriptor, followed by a new line | ✔️ |
| ft_putnbr_fd | Outputs a number to a file descriptor. | ✔️ |

## Bonus Functions

|      Function Name      | Description |      Status       |
|--------------|----|:---------------:|
|   ft_lstnew    | Creates a new node. |   ✔️   | 
| ft_lstadd_front | Adds a node to the beginning of the list. |  ✔️    |
|   ft_lstsize   | Counts the number of nodes in a list. |  ✔️    | 
| ft_lstlast    | Returns the last node of the list. |   ✔️  |
| ft_lstadd_back | Adds a node at the end of a list. |    ✔️  | 
| ft_lstdelone   | Deletes and frees a node of the list. |  ✔️   |
|  ft_lstclear   | Deletes and clear the list. |   ✔️   | 
| ft_lstiter  | Applies a function to each node of the list. |    ✔️  |
| ft_lstmap         | Applies a function to each node of the list, and creates a new list from the results of the function applied. |  ✔️    |

# The Norm

The norm is set of rules stipulated by 42 for the pedagogical needs of the school. It enforces these rules through an open source tool called "Norminette", which the students can run to check if their code is complaint. Some of these rules are:

```
- No for, do...while, switch, case, goto, ternary operators and variable-length arrays are allowed
- Each function must be a maximum of 25 lines, not counting the function's curly brackets
- Each line must be at most 80 columns wide, comments included
- A function can take 4 named parameters maximum
- No assigns and declarations in the same line (unless static)
- You can't declare more than 5 variables per function
- 4 space tabulations
- and so on...
```
- [Norminette](https://github.com/42School/norminette) - The tool to enforce the 42 style of coding.
- [42 Header](https://github.com/42Paris/42header) - The header used by 42. To be used with Vim.
