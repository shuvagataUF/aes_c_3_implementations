# aes_c_3_implementations

This repository contains three implementations of AES in C. This is used in our computer architecture project. The implementations are to be run in ARM64 architecture.

The links for the implementations are given below:
1. [tiny-aes-c](https://github.com/kokke/tiny-AES-c)
2. [aes-in-c](https://github.com/m3y54m/aes-in-c)
3. [AES](https://github.com/dhuertas/AES)

# Build the code

The compiled binaries are already there inside the **build** directory for associated AES implementations.

To build the code yourself, go into the directory of the implementations you want to use, then run
```
make
```
or
```
make all
```
This will create a **build** directory (if not created beforehand) and place the compiled binary inside that directory.

# Running the code

The code is built for **ARM** architecture, so it can't be run in an **x86** computer. The binaries are to be loaded to the simulated **Ubuntu** running on **ARM** architecture for execution.
