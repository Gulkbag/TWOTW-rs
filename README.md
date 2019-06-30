`Please if you get offended easily don't play this game`

# Manual
you can find the manual for this game [Here](https://gulkbag.github.io/TWOTW-Man/)

# Why rust?

Rust is a systems programming language targeting roughly the same space as C++. That means it’s fast and is generally used for things where you need a fair bit of control over how are things structured in memory, etc. Rust is a good candidate for writing a browser, database, operating system, web server and…​ games.

What made me like Rust is that it's pretty low level so i could use it for stuff i would normally go for C for, with good support for calling into libs written in C/C++, it's a language that lets you write clean code but in the same time use low level stuff (C is still the best tho lmao its' my favorite language).

# Libraries

Why libtcod? it's a library that's simple and specially written for rougelikes, it gives me everything i need to make a rougelike

`NOTE: libtcod originally was a C++ library and has a python version, but i am using for this the rust binding tcod-rs`

`NOTE: please don't use the code for this game as a refrence, it can be improved by a ton and made with more care and more better coding practices`

### Building on Linux

Run the equivalent of:

```sh
$ sudo apt-get install gcc g++ make libsdl2-dev
$ cd TWOTW
$ cargo build --release
$ cargo run --release
```

on your distro.

### Building on Windows (with MSVC)

Make sure you have Visual Studio 2013 or later **with the C++ tools
option** installed. You also need the "MSVC ABI" version of the Rust
compiler (as opposed to the "GNU ABI" one).

Then, set up the compilation environment, make sure Rust is in your
`PATH` and run Cargo:

```
C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\vcvarsall.bat amd64
set PATH=%PATH%;C:\Program Files (x86)\Rust\bin
cd TWOTW
cargo build --release
cargo run --release
```


### Building on Windows (with MinGW)

You have to [download and install MinGW](http://www.mingw.org/). Then,
add Rust's and MinGW's bin directories to your path and compile the game:

```
set PATH=%PATH%;C:\Program Files (x86)\Rust\bin;C:\MinGW\bin
cd TWOTW
cargo build --release
cargo run --release
```


### Building on Mac OS X

1. [Install Homebrew](http://brew.sh/)
2. Run:

```sh
$ brew install pkg-config sdl2
$ cd TWOTW
$ cargo build --release
$ cargo run --release
```
--------

### Using existing binary distribution

Right now we have only windows binaries, arch, void and gentoo linux binaries and Mac are in progress, you can find all in the releases section.

# License
**tcod-rs** is licensed under [WTFPL v2](http://www.wtfpl.net/txt/copying/). See `LICENSE` for the full text of the license (don't worry -- it's really short and to the point).
