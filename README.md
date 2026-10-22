# SnakeGame

A classic Snake game implemented in C using the `ncurses` library.

## Requirements

Before compiling the game, install the following dependencies:

- `gcc` — C compiler
- `libncurses5-dev` — ncurses development files
- `libncursesw5-dev` — wide-character ncurses development files

### Install on Debian / Ubuntu

```bash
sudo apt update
sudo apt install gcc libncurses5-dev libncursesw5-dev
```

## Compilation

Compile the source files using GCC:

```bash
gcc -o snake screen.h list.h list.c screen.c main.c -lncurses
```

## Execution

Run the compiled executable:

```bash
./snake
```

## Project Structure

```text
SnakeGame/
├── main.c
├── screen.c
├── screen.h
├── list.c
└── list.h
```

## Troubleshooting

### Missing ncurses headers

If compilation fails because `ncurses.h` cannot be found, verify that the ncurses development packages are installed.

### Linker errors

If GCC reports unresolved ncurses symbols, check that the ncurses libraries are installed and that `-lncurses` appears after the source files in the compilation command.

### Executable permission

If necessary, make the compiled executable runnable:

```bash
chmod +x snake
./snake
```

## License

No license has been specified in this README. Check the repository for an existing `LICENSE` file before distributing or modifying the project.

---

**SnakeGame** — A classic game built with C and ncurses.
