# Libft
**What is Libft?**

This project is about understanding how functions of the standard C library work, re-code them and create my own library, which will be used in the future projects.

**Requirements:**
- All functions must have the same prototypes and behave like original ones
- Only 3 standart C library functions allowed: write(), malloc(), free()
- Code must be written according C98 standart
- Everything must compile with the flags -std=c98 -Wall -Wextra -Werror
- Code must comply with the norminette rules. The norminette  is a programming standard that defines a set of rules to follow. Its repository is available at https://github.com/42School/norminette. Some of the rules are:
  - Each function must be maximum 25 lines, not counting the function's own curly brackets.
  - Each line must be at most 80 columns wide, comments included.
  - A function can take 4 named parameters maximum.
  - You can't declare more than 5 variables per function.
  - You're not allowed to use: for , do...while , switch , case ,  goto  , ternary operators such as `?' and VLAs - Variable Length Arrays.

**Project related documents:**
- [Subject pdf](https://github.com/VMiseikis/Libft/blob/master/docs/libft.en.subject.pdf) - function descriptions and prototypes. General requirements.</br>
- [Normintte rules](https://github.com/VMiseikis/Libft/blob/master/docs/en.norm.pdf) - more detailed documentation of norminete rules.

## Usage

Clone repository:
```
git clone https://github.com/VMiseikis/Libft.git libft
```

Enter cloned directory:
```
cd libft
```

Create library archive:
```
make
```

Add header to your .c files and use the Libft functions:
```
#include "libft.h"
```

Compile your program and link it with the library:
```
gcc -o my_program main.c -I./includes -L. -lft
```
  - ```I./includes```: Tells the compiler where to find the header files.
  - ```L.```: Tells the linker where to find the library file (libft.a is in the current directory).
  - ```lft```: Specifies the library to link with (without the lib prefix and the .a extension).

Run your program:
```
./my_program
```

## Implemented functions:

#### Functions from <ctype.h>
	
• `ft_isalpha` - checks for an alphabetic character.
	
• `ft_isdigit` - checks for a digit (0 through 9).
	
• `ft_isalnum` - checks for an alphanumeric character.
	
• `ft_isascii` - checks whether c fits into the ASCII character set.
	
• `ft_isprint` - checks for any printable character.
	
• `ft_toupper` - convert char to uppercase.

• `ft_tolower` - convert char to lowercase.
	
#### Functions from <string.h>
	
• `ft_memset`   - fill memory with a constant byte.
	
• `ft_strlen`   - calculate the length of a string.
	
• `t_bzero`     - zero a byte string.
	
• `ft_memcpy`   - copy memory area.
	
• `ft_memmove`  - copy memory area.
	
• `ft_strlcpy`  - copy string to an specific size.
	
• `ft_strlcat`  - concatenate string to an specific size.
	
• `ft_strchr`   - locate character in string.
	
• `ft_strrchr`  - locate character in string.
	
• `ft_strncmp`  - compare two strings.
	
• `ft_memchr`   - scan memory for a character.
	
• `ft_memcmp`   - compare memory areas.
	
• `ft_strnstr`  - locate a substring in a string.
	
• `ft_strdup`   - creates a dupplicate for the string passed as parameter.
	
#### Functions from <stdlib.h>
	
• `ft_atoi`    - convert a string to an integer.
	
• `ft_calloc`  - allocates memory and sets its bytes' values to 0.
	
#### Non-standard functions
	
• `ft_substr` - returns a substring from a string.
	
• `ft_strjoin` - concatenates two strings.
	
• `ft_strtrim` - trims the beginning and end of string with specific set of chars.
	
• `ft_split` - splits a string using a char as parameter.
	
• `ft_itoa` - converts a number into a string.
	
• `ft_strmapi` - applies a function to each character of a string.
	
• `ft_striteri` - applies a function to each character of a string.
	
• `ft_putchar_fd` - output a char to a file descriptor.
	
• `ft_putstr_fd` - output a string to a file descriptor.
	
• `ft_putendl_fd` - output a string to a file descriptor, followed by a new line.
	
• `ft_putnbr_fd` - output a number to a file descriptor.
	
#### Linked list functions
	
• `ft_lstnew` - creates a new list element.
	
• `ft_lstadd_front` - adds an element at the beginning of a list.
	
• `ft_lstsize` - counts the number of elements in a list.
	
• `ft_lstlast` - returns the last element of the list.
	
• `ft_lstadd_back` - adds an element at the end of a list.
	
• `ft_lstclear` - deletes and free list.

• `ft_lstiter` - applies a function to each element of a list.
	
• `ft_lstmap` - applies a function to each element of a list.

## Recources
- [Linux man pages](https://linux.die.net/man/)

## Testers
Tester used to check the project.
- [Libft unit tester](https://github.com/alelievr/libft-unit-test)
- [Libft war machine tester](https://github.com/ska42/libft-war-machine)

