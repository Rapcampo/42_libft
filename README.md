# Table of contents
- [Overview](#overview)
  * [written in C and accordance with the norm](#written-in-c-and-accordance-with-the-norm)
  * [Mandatory part:](#mandatory-part)
  * [Technical considerations:](#technical-considerations)
  * [Functions to be included:](#functions-to-be-included)
  * [Mandatory functions](#mandatory-functions)
  * [Bonus Functions](#bonus-functions)
- [Function Breakdown](#function-breakdown)

# Overview

This is the first project of the common core for the 42 programming school, as such it follow  general guidelines that must be complient with the school norms for readability of the code. The following are the general rules for this project.

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

## Mandatory functions

| **Libc** | Done | ***not libc*** | done | **Libc** | Done | ***not libc*** | done | **Libc** | Done |
|:--------:|:----:|:--------------:|:----:|:--------:|:----:|:--------------:|:----:|:--------:|:----:|
| isalpha  |  ✔️  |   ft_substr    |  ✔️  |  bzero   |  ✔️  | ft_putchar_fd  |  ✔️  |  strchr  |  ✔️  |
| isdigit  |  ✔️  |   ft_strjoin   |  ✔️  |  memcpy  |  ✔️  |  ft_putstr_fd  |  ✔️  | strrchr  |  ✔️  |
| isalnum  |  ✔️  |   ft_strtrim   |  ✔️  | memmove  |  ✔️  | ft_putendl_fd  |  ✔️  | strncmp  |  ✔️  |
| isascii  |  ✔️  |    ft_split   |  ✔️  | strlcpy  |  ✔️  |  ft_putnbr_fd  |  ✔️  |  memchr  |  ✔️  |
| isprint  |  ✔️  |    ft_itoa     |  ✔️  | strlcat  |  ✔️  |                |      |  memcmp  |  ✔️  |
| strlen  |  ✔️  |   ft_strmapi   |  ✔️  | toupper  |  ✔️  |                |      |   atoi   |  ✔️  |
|  memset  |  ✔️  |  ft_striteri   |  ✔️  | tolower  |  ✔️  |                |      |  Calloc  |  ✔️  |
|  strdup  |  ✔️  |                |      | strnstr |  ✔️  |                |      |          |      |

## Bonus Functions

|      Func      | Done |      Func       | Done |
|:--------------:|:----:|:---------------:|:----:|
|   ft_lstnew    |   ✔️   | ft_lstadd_front |  ✔️    |
|   ft_lstsize   |  ✔️    |   ft_lstlast    |    ✔️  |
| ft_lstadd_back |    ✔️  |  ft_lstdelone   |   ✔️   |
|  ft_lstclear   |   ✔️   |   ft_lstiter    |    ✔️  |
| ft_lstmap              |  ✔️    |                 |      |

# Function Breakdown

For each function there will be a brief description with a link to a detailed wiki style overview of how the function works. This detailed description is done with the porpuse of a better understanding of how each of this function works as well as the structure of their syntax. 

isaplha - 
