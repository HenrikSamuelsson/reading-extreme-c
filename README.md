# Reading Extreme C

Notes taken by reading the book Extreme C, written by Kamran Amini (Packt Publishing October 2019).

## About the Book

This book is not an beginners C programming book. If you have never done any programming before you will need to get some prior experience before reading this book. Can for example read one or two introductory C programming books first, and then get back to this book to take your C skills to the next level.

## Chapter 1 - Essential Features

First chapter discusses a small selection of C features. Many of these features are a little more advanced and will in introductory books typically just be briefly explained. The strategy used in this book is to intentionally leave out much content on C basics and instead include coverage of more advanced features.

### Preprocessor Directives

The C preprocessor implements the macro language used to transform C, C++, and Objective-C programs before they are compiled. It can also be useful on its own.

The source code will typically be altered by the preprocessor, but remains in a human readable text format.

A notable resource, to learn more, about the preprocessor is the [GCC CPP Manual](https://gcc.gnu.org/onlinedocs/gcc-13.2.0/cpp/). Note that CPP in this context stands for C preprocessor, and not C++.

### Variable Pointers

### Some Details About Functions

### Function Pointers

### Structures

## Chapter 3 - Object Files

### Section 3.2 Object File Formats

An object file is a work product that is output from the compiler. The object file will depend on the platform for which the program is compiled. The platform dependencies will include the processor instruction set but there can then be other dependencies such as the available systems call to an underlying operating system.

![object-file-formats](https://github.com/HenrikSamuelsson/reading-extreme-c/assets/5353030/233eff56-d127-4ef7-8f49-3351de5533bd)

*Figure: Family three of some object file formats.*

The above figure shows the evolvement of objects file formats. First there was assembler output (a.out) which evolved into Common Object File Format (COFF). Then more recently there is Portable Execution (PE) for Windows, Mach-O for Apple OS/X, and Executable and Linkable Format (ELF) for Unix. Note that ELF is not limited to UNIX since it is cross platform and is for example commonly used in embedded systems.

### Section 3.6 Static Libraries

Static libraries can be created and then be shared by more than one executables. Static libraries are part of the executable, the linker puts everything found in the given relocatable files into the final executable file. In other words, the linker detects the undefined symbols, and required definitions, and tries to find them in the given relocatable object files, then puts them all in the output executable file. The executable will be self contained.
