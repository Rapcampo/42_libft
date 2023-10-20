### overview

### written in C and accordance with the norm  
- error free, no seg fault, bus error, double free... undefined is ok, if it happens once. 
- no memory leaks! always free heap memory properly!  
- must submit a makefile if required, the make file must compile with the usual flags Werror, Wextra, Wall, no relinks.  
- must contain the rules $(name), all, clean, fclean and re.  
- if bonuses are wanted, must include a rule in the makefile.  
- bonuses must be in a different file "bonus.c or bonus.h"  if your project allows you to use your libft folder with its makefile. your project makefile must compile the library by using its makefile then the project.  
- encourage to create your own test programs, during the defence you are allowed to use your tests and the tests of the peers you evaluated.  

## Mandatory part:  
 
 - files: makefile, libft.h, ft_*.c 
 - makefile: NAME, all, clean, fclean, re.  
 - external functions  
 - write your own library: a collection of useful functions that will be a useful tool for your cursus  
   
## technical considerations:  
 
- declaring global variables is forbidden.  
- if you need helper functions to split a more complex function, they must be defined as static. so their scope becomes limited to the appropriate file. 
- place all the files at the root of the repository.  
- unused files are forbidden.  
- every .c file must be compiled with the flags -Wall -Wextra -Werror.  
- must use the command ar to create your library. using libtool is forbidden.  
 - your libft.a has to be created at the root of your repository.  
   
## Functions to be included:  
- redo a set of libc functions. same prototype, same behaviours. only difference must be their names.  
- they must use the ft_ prefix.
# concepts:

## Mandatory functions

| **Libc** | Done | ***not libc*** | done | **Libc** | Done | ***not libc*** | done | **Libc** | Done |
|:--------:|:----:|:--------------:|:----:|:--------:|:----:|:--------------:|:----:|:--------:|:----:|
| [[isalpha]]  |  ✔️  |   [[ft_substr]]    |  ✔️  |  [[bzero]]   |  ✔️  | [[ft_putchar_fd]]  |  ✔️  |  [[strchr]]  |  ✔️  |
| [[isdigit]]  |  ✔️  |   [[ft_strjoin]]   |  ✔️  |  [[memcpy]]  |  ✔️  |  [[ft_putstr_fd]]  |  ✔️  | [[strrchr]]  |  ✔️  |
| [[isalnum]]  |  ✔️  |   [[ft_strtrim]]   |  ✔️  | [[memmove]]  |  ✔️  | [[ft_putendl_fd]]  |  ✔️  | [[strncmp]]  |  ✔️  |
| [[isascii]]  |  ✔️  |    [[ft_split]]    |  ✔️  | [[strlcpy]]  |  ✔️  |  [[ft_putnbr_fd]]  |  ✔️  |  [[memchr]]  |  ✔️  |
| [[isprint]]  |  ✔️  |    [[ft_itoa]]     |  ✔️  | [[strlcat]]  |  ✔️  |                |      |  [[memcmp]]  |  ✔️  |
|  [[strlen]]  |  ✔️  |   [[ft_strmapi]]   |  ✔️  | [[toupper]]  |  ✔️  |                |      |   [[atoi]]   |  ✔️  |
|  [[memset]]  |  ✔️  |  [[ft_striteri]]   |  ✔️  | [[tolower]]  |  ✔️  |                |      |  [[Calloc]]  |  ✔️  |
|  [[strdup]]  |  ✔️  |                |      | [[strnstr]] |  ✔️  |                |      |          |      |

## Bonus Functions

|      Func      | Done |      Func       | Done |
|:--------------:|:----:|:---------------:|:----:|
|   [[ft_lstnew]]    |   ✔️   | [[ft_lstadd_front]] |  ✔️    |
|   [[ft_lstsize]]   |  ✔️    |   [[ft_lstlast]]    |    ✔️  |
| [[ft_lstadd_back]] |    ✔️  |  [[ft_lstdelone]]   |   ✔️   |
|  [[ft_lstclear]]   |   ✔️   |   [[ft_lstiter]]    |    ✔️  |
| [[ft_lstmap ]]              |  ✔️    |                 |      |

 - [x] basic functions for libft 🔼 📅 2023-10-08 ✅ 2023-10-08
 - [x] Bonus functions ⏫ 📅 2023-10-15 ✅ 2023-10-12

- ## [[makefile]] 
- [/] watch makefile tutorial by Nuno 🔼
- [/] read make-a-make
- [x] makefile 🔺 📅 2023-10-13 ✅ 2023-10-12
- [x] Start bonuses 🔼 ✅ 2023-10-15
- [x] review code and make wiki 🔺 📅 2023-10-15 ✅ 2023-10-15
- [x] finish bonuses and deliver project 🔺 📅 2023-10-15 ✅ 2023-10-15