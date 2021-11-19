# 42_libft
## About
The first proyect of 42 cursus: creating a library with some functions that will be useful later on.
This repository contains the .and .h files as well as the Makefile used for the proyect libft in 42 Madrid, November 2021 (Final mark: 125/100).
I do not condone cheating or plagiarism, so do **NOT copy** my code to validate any other libft proyects, thank you.
If you have any questions about the code please contact me in slack (username: samoreno), I usually answer quickly.

My 42 intra profile: https://profile.intra.42.fr/users/samoreno

## Files

### Mandatory part

#### Libc functions
| File name    | Description | Other |
| ---------    | ----------- | ---- |
| ft_isalpha.c | Takes an integer and returns 1 if it's alphabetical and 0 if not (in ascii).                                                            | See: man isalpha |
| ft_isdigit.c | Takes an integer and returns 1 if it's a digit (0-9) and 0 if not (in ascii).                                                           | See: man isdigit |
| ft_isalnum.c | Takes an integer and returns 1 if it's alphabetical or a digit (0-9) and 0 if not (in ascii).                                           | See: man isalnum |
| ft_isascii.c | Takes an integer and returns 1 if it is in the ascii table and 0 if not.                                                                | See: man isascii |
| ft_isprint.c | Takes an integer and returns 1 if it's a printable character and 0 if not (in ascii).                                                   | See: man isalpha |
| ft_strlen .c | Takes an array of characters _s_ and returns it's length (Null not included).                                                           | See: man strlen  |
| ft_memset.c  | Copies the character _c_ to the first _n_ characters of the string pointed to, by the argument _b_.                                     | See: man memset  |
| ft_bzero.c   | Erases the data in the _n_ bytes of the memory starting at the location pointed to by _s_, by writing '\0'.                             | See: man bzero   |
| ft_memcpy.c  | Copies n characters from memory area _src_ to memory area _dest_.                                                                       | See: man memcpy  |
| ft_memmove.c | Does the same as memcpy but for overlapping memory blocks, memmove is a safer approach than memcpy.                       | See: ft_memcpy and man memmove |
| ft_strlcpy.c | Copies up to _size - 1_ characters from _src_ to _dst_ NUL-terminating the result. Returns the length of the string it tried to create. | See: man strlcpy |
| ft_strlcat.c | Appends _src_ to the end of _dst_. It will append _size - strlen(dst) - 1_ bytes, NUL-terminating the result. Returns the length of the string it tried to create unless it traverses size characters without finding a NUL. Then the length of the string is considered to be size and the destination string will not be NUL-terminated| See: man strlcat |
| ft_toupper.c | Takes a character and returns it in uppercase if it was a lowercase alphabetical character. Else it returns it unmodified.              | See: man toupper |
| ft_tolower.c | Takes a character and returns it in lowercase if it was an uppercase alphabetical character. Else it returns it unmodified.             | See: man tolower |
| ft_strchr.c  | Searches for the first occurrence of the character _c_ in the string pointed to by the argument _s_. It uses _c_ as an unsigned char.   | See: man strchr  |
| ft_strrchr.c | Searches for the last occurrence of the character _c_ in the string pointed to by the argument _s_. It uses _c_ as an unsigned char.    | See: man strrchr |
| ft_strncmp.c | Compares one by one at most the first _n_ bytes of _str1_ and _str2_. When it finds two different characters it returns the difference (char of _str1_ - char of _str2_) in ascii. | See: man strncmp |
| ft_memchr.c  | Searches for the first occurrence of _c_ in the first _n_ bytes of _s_. It uses _c_ as an unsigned char.                                | See: man memchr  |
| ft_memcmp.c  | Does the same as strncmp but it uses memory areas isntead of strings                                                                    | See: ft_strncmp and man memcmp |
| ft_strnstr.c | Locates the first occurrence of the	_needle_ in _haystack_, where not more than	_len_ characters are searched. Characters that appear after a '\0' character are not searched. If	_needle_ is an empty string, _haystack_ is returned; if _needle_ occurs nowhere in _haystack_, NULL is returned; otherwise a pointer to the first	character of the first occurrence of _needle_ is returned.	 | See: man strnstr |
| ft_atoi.c   | Converts _str_ to an integer. If no valid conversion could be performed, it returns zero. It ignores all spaces as concieved by isspace. | See: man atoi and man isspace|
| ft_calloc.c | Allocates the requested memory and returns a pointer to it. It sets allocated memory to zero.                                            | See: man calloc and man malloc |
| ft_strdup.c | Returns a pointer to a new string that is a copy of _s_.  Memory for the new string is allocated with malloc.                             | See: man strdup and man malloc |

#### Additional functions
| File name    | Description | Other |
| ---------    | ----------- | ---- |
| ft_substr.c  | Allocates with malloc and returns a substring from the string _s_. The substring begins at index _start_ and is of maximum size _len_. | See: man malloc |
| ft_strjoin.c | Allocates with malloc and returns a new string, which is the result of the concatenation of _s1_ and _s2_.                             | See: man malloc |
| ft_strtrim.c | Allocates with malloc and returns a copy of _s1_ with the characters specified in _set_ removed from the beginning and the end of the string. | See: man malloc |
| ft_split.c | Allocates with malloc and returns an array of strings obtained by splitting _s_ using the character _c_ as a delimiter. The array must be ended by a NULL pointer. | See: man malloc and man free|
| ft_itoa.c |  Allocates with malloc and returns a string representing the integer received as an argument.Negative numbers must be handled.             | See: man malloc |
| ft_strmapi .c | Applies the function _f_ to each character of the string _s_ , and passing its index as first argument to create a new string with malloc resulting from successive applications of _f_. | See: man malloc |
| ft_striteri.c  | Applies the function _f_ to each character of the string _s_ , and passing its index as first argument. Each character is passed by address to f to be modified if necessary. |  |
| ft_putchar_fd.c | Outputs the character _c_ to the given file descriptor. | See: man write |
| ft_putstr_fd.c | Outputs the string _s_ to the given file descriptor. | See: man write |
| ft_putendl_fd.c | Outputs the string _s_ to the given file descriptor, followed by a newline. | See: man write |
| ft_putnbr_fd.c | Outputs the integer _n_ to the given file descriptor. | See: man write |

### Bonus part
| File name    | Description | Other |
| ---------    | ----------- | ---- |
| ft_lstnew.c  | Allocates with malloc and returns a new element. The variable _content_ is initialized with the value of the parameter _content_. The variable _next_ is initialized to NULL. | See: man malloc |
| ft_lstadd_front.c | Adds the element _new_ at the beginning of the list. | |
| ft_lstsize.c | Counts the number of elements in a list. | |
| ft_lstlast.c | Returns the last element of the list. | |
| ft_lstadd_back.c | Adds the element _new_ at the end of the list. | |
| ft_lstdelone.c |Takes as a parameter an element and frees the memory of the element’s content using the function _del_ given as a parameter and free the element. The memory of _next_ must not be freed. | See: man free |
| ft_lstclear.c | Deletes and frees the given element and every successor of that element, using the function _del_ and free. Finally, the pointer to the list must be set to NULL. | See: man free |
| ft_lstiter.c | Iterates the list _lst_ and applies the function _f_ to the content of each element. | |
| ft_lstiter.c | Iterates the list _lst_ and applies the function _f_ to the content of each element. Creates a new list resulting of the successive applications of the function _f_. The _del_ function is used to delete the content of an element if needed. | See: man malloc and man free |
