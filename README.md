Mach Sieve
---

An implementation of the Sieve of Eratosthenes in Mach.
It is not meant to be a useful or efficient implementation, but rather a demonstration of the basic features of the Mach programming language.

This project demonstrates the intended structure of a Mach project, including the use of dependencies (of which the standard library is one).

# Building

You need the `mach` compiler. Install the latest [release](https://github.com/octalide/mach/releases) and ensure it is on your `PATH`.

Clone the repository:

```bash
git clone https://github.com/octalide/mach-sieve
cd mach-sieve
```

Fetch the standard library dependency:

```bash
mach dep pull
```

Build the project:

```bash
mach build .
```

This compiles the source files and places the resulting binary in `out/linux/bin/sieve`.

You can also build and run in one step. Arguments after `--` are forwarded to the program:

```bash
mach run .          # sieve up to the default limit
mach run . -- 1000  # sieve up to 1000
```
