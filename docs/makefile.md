# Makefile notes

[Home](index.html)

A `Makefile` describes how to build a program. You run it with `make`.

## A small example

```make
main: main.c
	gcc main.c -o main

clean:
	rm -f main
```

## Things to remember

- Recipe lines start with a **Tab**, not spaces.
- `make main` builds the `main` target.
- `make clean` runs the `clean` target.
- If a file named `clean` exists, `make clean` says it is up to date, unless `clean` is declared with `.PHONY`.

Useful link: [GNU make manual](https://www.gnu.org/software/make/manual/make.html)
