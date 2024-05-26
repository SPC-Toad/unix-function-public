# Project Overview

This project consists of tools for examining sections and symbols of object files. The tools implement functionalities similar to `objdump -h` and `nm` commands. There are both static and dynamic library versions of these tools available.

## Demo video

https://github.com/SPC-Toad/unix-function-public/assets/111462911/7f80847d-a118-48fa-8295-71cacba36351




## Want to view how I implemented it?
    Please contact me seperately. I will give you access to my private repository where the code is. 

        - Please inform me who you are and why you want to access it. Thank you!

## Tools

### Static Library Versions

1. **getsections**
   - Implements `objdump -h` functionality.
   - Usage: `./getsections <object-file>`

2. **getsyms**
   - Implements `nm` functionality.
   - Usage: `./getsyms <object-file>`

### Dynamic Library Versions

1. **getsections_dl**
   - Dynamic library version of `getsections`.
   - Usage: `./getsections_dl <object-file>`

2. **getsyms_dl**
   - Dynamic library version of `getsyms`.
   - Usage: `./getsyms_dl <object-file>`

## Additional Files

- **objcopy.c**
  - Source file related to object copying functionality.
  
- **objsect.c**
  - Source file related to section handling in object files.
  
- **objsym.c**
  - Source file related to symbol handling in object files.
  
- **Makefile**
  - Build script to compile the project.

## Compilation

To compile the project, use the provided `Makefile`. Simply run the following command in the project directory:

```bash
make
```

This will generate the executables for the static and dynamic library versions of the tools.

## Usage

To use any of the tools, run the corresponding executable with the object file as an argument. For example:

```bash
./getsections example.o
./getsyms example.o
./getsections_dl example.o
./getsyms_dl example.o
```

These commands will print out the sections and symbols of the provided object file respectively.
