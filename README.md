# :books: Libft ![Static Badge](https://img.shields.io/badge/Barcelona-black?style=for-the-badge&logo=42&logoColor=%23FFFFFF)
![Static Badge](https://img.shields.io/badge/c-grey?style=flat&logo=c)
![Static Badge](https://img.shields.io/badge/Makefile-green?style=flat&logo=AnkerMake)
![Static Badge](https://img.shields.io/badge/status-completed-green?style=flat)


The first project in the 42 syllabus. A simple C library with useful functions for future projects.

## :hammer: Compilation
Firstly, copy the repository into you computer directory:

```bash
git clone https://github.com/alexpg7/Libft.git Libft 
```

Once copied, just execute the `make` command:

```bash
make
```

The `make`command should output all the object files (`*.o`) and the `libft.a` file.

## :book: How to use it

The library can be used in any project adding the `libft.h` header and including `libft.a` in the compilation. Example:

```bash
cc main.c file_1.c ... file_n.c libft.a
```

## :bookmark_tabs: Documentation

The function prototypes with a simple description.

### :eye: ``get_next_line``
* ``char	*get_next_line(int fd);`` 

  Returns the next line (ended in `\n`) of a file described by `fd`.
This function belongs originally to an independent project ([get_next_line](https://github.com/alexpg7/get_next_line)).

### :books: Libft
* ``void	ft_bzero(void *s, size_t n);``

  Writes `n` zero-valued bytes into `s`.

* ``int		ft_isalpha(int c);``

  Returns `1` if `c` is alphabetic. Otherwise, it returns `1`.

* ``int		ft_isdigit(int c);``

  Returns `1` if `c` is numeric. Otherwise, it returns `1`.

* ``int		ft_isalnum(int c);``

  Returns `1` if `c` is alphanumeric. Otherwise, it returns `1`.

* ``int		ft_isalnum2(int c);``

  Works exactly like `ft_isalnum` but includes the `_` character. (useful for [minishell](https://github.com/alexpg7/minishell_alpascua_ineiras-))

* ``int		ft_isascii(int c);``

  Returns `1` if `c` belongs to the ASCII code. Otherwise, it returns `1`.

* ``int		ft_isprint(int c);``

  Returns `1` if `c` is a printable character. Otherwise, it returns `1`.

* ``void	*ft_memcpy(void *dest, const void *src, size_t n);``

  Copies `n` bytes from `src` to `dest`.

* ``void	*ft_memmove(void *dest, const void *src, size_t n);``

  Works the same as `ft_memcpy` but avoids overlaping between memory spaces.

* ``void	*ft_memchr(const void *s, int c, size_t n);``

  Returns the first appearence of `c` in `s` (from left to right). If it fails, it returns `NULL`. `n` is the number of bytes to be searched.

* ``int		ft_memcmp(const void *s1, const void *s2, size_t n);``

  Compares the first `n` bytes of `s1` and `s2` and returns the difference of the first different one.

* ``void	*ft_memset(void *s, int c, size_t n);``

  Sets `n` bytes of `s` to the `c` value.

* ``size_t	ft_strlcpy(char *dst, const char *src, size_t size);``

  Copies `src` into `dest` with size `size`, null-terminating the last byte.

* ``size_t	ft_strlcat(char *dst, const char *src, size_t size);``

  Concatenates `src` at the end of `dest`, null-terminating the last byte.

* ``size_t	ft_strlen(const char *s);``

  Returns the length of a string.

* ``int		ft_toupper(int c);``

  Sets the `c` character to uppercase (if it is alphabetic).

* ``int		ft_tolower(int c);``

  Sets the `c` character to lowercase (if it is alphabetic).

* ``char	*ft_strchr(const char *s, int c);``

  Returns the first appearence of `c` in `s` (from left to right). If it fails, it returns `NULL`.

* ``char	*ft_strrchr(const char *s, int c);``

  Returns the first appearence of `c` in `s` (from right to left). If it fails, it returns `NULL`.

* ``int		ft_strncmp(const char *s1, const char *s2, size_t n);``

  Compares the first `n` characters of `s1` and `s2` and returns the difference of the first different one.

* ``int		ft_strcmp(const char *s1, const char *s2);``

  Compares the characters of `s1` and `s2` and returns the difference of the first different one.

* ``char	*ft_strnstr(const char *big, const char *little, size_t len);``

  Search for the first appearence of `little` in `big`. If it fails, it returns `NULL`.

* ``int		ft_atoi(const char *nptr);``

  Returns the integer value of the string `nptr`, with formating freedom. Example: (char *)("   ++-+--42") $\rightarrow$ (int)(-42).

* ``double	ft_atof(const char *str);``

  Returns the float value of the string `str`.

* ``void	*ft_calloc(size_t nmemb, size_t size);``

  Calls `malloc` with size `nmeb * size`. If `malloc` fails, sets the memory tried to allocate to `\0`.

* ``char	*ft_strdup(const char *s);``

  Returns a copy of `s`.

* ``char	*ft_substr(char const *s, unsigned int start, size_t len);``

  Returns a substring of `s` starting in the `start` byte with size `len`.

* ``char	*ft_strjoin(char const *s1, char const *s2);``

  Joins `s1` and `s2` into a single string.

* ``char	*ft_strjoin3(char const *s1, char const *s2, char const *s3);``

  Joins `s1`, `s2` and `s3` into a single string.

* ``int		ft_freestrarr(char ***array, int ret);``

  Frees the string array pointed by `array` and returns `ret`.

* ``char	*ft_strtrim(char const *s1, char const *set);``

  Removes the characters in `set` from the beggining and end of `s1`.

* ``char	**ft_split(char const *s, char c);``

  Creates an array of strings separating the "words" in `s` using the `c` separator.

* ``void	*ft_free(char **ptr, int i);``

  Frees the first `i` strings of the string array `ptr`.

* ``char	*ft_itoa(int n);``

  Returns a string made out of the `n` integer.

* ``char	*ft_strmapi(char const *s, char (*f)(unsigned int, char));``

  Applies the function `f` to each character of `s`, appends it into a new string and returns the result.

* ``void	ft_striteri(char *s, void (*f)(unsigned int, char *));``

  Applies the function `f` to the `s + i` string, where `i` is the `i`th character of `s`, appends it into a new string and returns the result.

* ``int		ft_putchar_fd(char c, int fd);``

  Writes the character `c` into the `fd` file descriptor.

* ``int		ft_putstr_fd(char *s, int fd);``

  Writes the `s` string into the `fd` file descriptor.

* ``void	ft_putendl_fd(char *s, int fd);``

  Writes the `s` string into the `fd` file descriptor, ending ot with `\n`.

* ``void	ft_putnbr_fd(int n, int fd);``

  Writes the number `n` (in base 10) into the `fd` file descriptor.

### :heavy_plus_sign: Libft  $\color{green}{\textsf{Bonus}}$

This includes a new struct, useful for creating noded lists:

```C
typedef struct s_list
{
	void		*content;
	struct s_list	*next;
}	t_list;
```

* ``t_list	*ft_lstnew(void *content);``

  Creates a new node filled with `content`.

* ``void	ft_lstadd_front(t_list **lst, t_list *new);``

  Adds a node `new` to the beginning of the list pointed by (the direction of the first element) `lst`.

* ``void	ft_lstadd_back(t_list **lst, t_list *new);``

  Adds a node `new` to the end of the list pointed by (the direction of the first element) `lst`.

* ``int		ft_lstsize(t_list *lst);``

  Returns the number of nodes in `lst`.

* ``t_list	*ft_lstlast(t_list *lst);``

  Returns the direction of the last node in `lst`.

* ``void	ft_lstdelone(t_list *lst, void (*del)(void *));``

  Deletes one element of `lst` freeing its content with `del`.

* ``void	ft_lstclear(t_list **lst, void (*del)(void *));``

  Frees the list `lst` and applies `del` to each element's content.

* ``void	ft_lstiter(t_list *lst, void (*f)(void *));``

  Applies the `f` function to each element of `lst`.

* ``t_list	*ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));``

  Maps the `f` function from every element in `lst` into a new list.

### :printer: ``ft_printf`` functions

These ones belong to an independent project ([ft_](https://github.com/alexpg7/ft_))

* ``int	ft_printf(char const *format, ...);``

  Works exactly the same as the original `printf` function but only accepts the `%c`, `%s`, `%p`, `%d`, `%i`, `%u`, `%x`, `%X` and `%%` formats.

* ``int	ft_printchar(char c);``

  Auxiliar function of ``ft_printf``.

* ``int	ft_printstr(char *str);``

* ``int	ft_numlen(unsigned long num, unsigned long base);``

  Auxiliar function of ``ft_printf``.

* ``int	ft_printbase(unsigned long nbr, char *base, unsigned long len);``

  Auxiliar function of ``ft_printf``.

* ``int	ft_printpointer(int long long ptr);``

  Auxiliar function of ``ft_printf``.
