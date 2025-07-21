# :books: Libft ![Static Badge](https://img.shields.io/badge/Barcelona-black?style=for-the-badge&logo=42&logoColor=%23FFFFFF)
![Static Badge](https://img.shields.io/badge/C-grey?style=flat)
![Static Badge](https://img.shields.io/badge/Makefile-green?style=flat)
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

``char	*get_next_line(int fd);`` 

Returns the next line (ended in `\n`) of a file described by `fd`.
This function belong originally to an independent project ([get_next_line](https://github.com/alexpg7/get_next_line))
