# libft
[![tclement's 42 Libft Score](https://badge42.vercel.app/api/v2/cl59lbrtc003009jqom2qgm4z/project/1898916)](https://github.com/JaeSeoKim/badge42)<br>
***This project creates a library with standard libc functions and several other generic functions, which will be used for other 42 projects.***

The purpose is to help us develop a deep understanding of the standard libc functions and how to use them. 

## Technical considerations

- Allowed functions: ```malloc```, ```free```, ```write```
- All heap allocated memory space must be properly freed when necessary

## Included functions

> libc functionss
* [ft_bzero](https://github.com/DelicaTessa/42-libft/blob/master/ft_bzero.c)
* [ft_calloc](https://github.com/DelicaTessa/42-libft/blob/master/ft_calloc.c)
* [ft_isalnum](https://github.com/DelicaTessa/42-libft/blob/master/ft_isalnum.c)
* [ft_isalpha](https://github.com/DelicaTessa/42-libft/blob/master/ft_isalpha.c)
* [ft_isascii](https://github.com/DelicaTessa/42-libft/blob/master/ft_isascii.c)
* [ft_isdigit](https://github.com/DelicaTessa/42-libft/blob/master/ft_isdigit.c)
* [ft_isprint](https://github.com/DelicaTessa/42-libft/blob/master/ft_isprint.c)
* [ft_itoa](https://github.com/DelicaTessa/42-libft/blob/master/ft_itoa.c)
* [ft_memccpy](https://github.com/DelicaTessa/42-libft/blob/master/ft_memccpy.c)
* [ft_memchr](https://github.com/DelicaTessa/42-libft/blob/master/ft_memchr.c)
* [ft_memcmp](https://github.com/DelicaTessa/42-libft/blob/master/ft_memcmp.c)
* [ft_memcpy](https://github.com/DelicaTessa/42-libft/blob/master/ft_memcpy.c)
* [ft_memmove](https://github.com/DelicaTessa/42-libft/blob/master/ft_memmove.c)
* [ft_memset](https://github.com/DelicaTessa/42-libft/blob/master/ft_memset.c)
* [ft_putchar_fd](https://github.com/DelicaTessa/42-libft/blob/master/ft_putchar_fd.c)
* [ft_putendl_fd](https://github.com/DelicaTessa/42-libft/blob/master/ft_putendl_fd.c)
* [ft_putnbr_fd](https://github.com/DelicaTessa/42-libft/blob/master/ft_putnbr_fd.c)
* [ft_tolower](https://github.com/DelicaTessa/42-libft/blob/master/ft_tolower.c)
* [ft_toupper](https://github.com/DelicaTessa/42-libft/blob/master/ft_substr.c)

> string manipulation
* [ft_atoi](https://github.com/DelicaTessa/42-libft/blob/master/ft_atoi.c)
* [ft_putstr_fd](https://github.com/DelicaTessa/42-libft/blob/master/ft_putstr_fd.c)
* [ft_split](https://github.com/DelicaTessa/42-libft/blob/master/ft_split.c)
* [ft_strchr](https://github.com/DelicaTessa/42-libft/blob/master/ft_strchr.c)
* [ft_strdup](https://github.com/DelicaTessa/42-libft/blob/master/ft_strdup.c)
* [ft_strjoin](https://github.com/DelicaTessa/42-libft/blob/master/ft_strjoin.c)
* [ft_strlcat](https://github.com/DelicaTessa/42-libft/blob/master/ft_strlcat.c)
* [ft_strlcpy](https://github.com/DelicaTessa/42-libft/blob/master/ft_strlcpy.c)
* [ft_strlen](https://github.com/DelicaTessa/42-libft/blob/master/ft_strlen.c)
* [ft_strmapi](https://github.com/DelicaTessa/42-libft/blob/master/ft_strmapi.c)
* [ft_strncmp](https://github.com/DelicaTessa/42-libft/blob/master/ft_strncmp.c)
* [ft_strnstr](https://github.com/DelicaTessa/42-libft/blob/master/ft_strnstr.c)
* [ft_strncmp](https://github.com/DelicaTessa/42-libft/blob/master/ft_strncmp.c)
* [ft_strrchr](https://github.com/DelicaTessa/42-libft/blob/master/ft_strrchr.c)
* [ft_strtrim](https://github.com/DelicaTessa/42-libft/blob/master/ft_strtrim.c)
* [ft_substr](https://github.com/DelicaTessa/42-libft/blob/master/ft_substr.c)

> linked list manipulation
* [ft_lstadd_back](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstadd_back_bonus.c)
* [ft_lstadd_front](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstadd_front_bonus.c)
* [ft_lstclear](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstclear_bonus.c)
* [ft_lstdelone](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstdelone_bonus.c)
* [ft_lstiter](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstiter_bonus.c)
* [ft_lstlast](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstlast_bonus.c)
* [ft_lstnew](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstnew_bonus.c)
* [ft_lstsize](https://github.com/DelicaTessa/42-libft/blob/master/ft_lstsize_bonus.c)

## How to test

> To test the library, create a ```test.c``` file to compile with the ```libft.a``` library

``` C
# include "libft.h"
# include <stdio.h>

int	main(void)
{
	char	*str;
	int	ret;

	str = "123456789";
	ret = ft_atoi(str);
	printf("ret is %d\n", ret);
	return (0);
}
```

> Run the commands below. You can replace the ```test.c``` with your own test file

``` shell
$ git clone https://github.com/DelicaTessa/42-libft.git
$ cd 42-libft
$ make
$ make bonus
$ gcc test.c libft.a
$ ./a.out
```

