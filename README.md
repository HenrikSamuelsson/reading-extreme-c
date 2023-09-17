# Reading Extreme C

Material related to reading the book Extreme C, written by Kamran Amini (Packt Publishing October 2019).

This book is not an beginners C programming book. If you have never done any C programming book you will need to read one or two introductory books first, to get some experience in C coding, and then get back to this book that will take your C skills to the next level.

## Notes on Chapter 1 - Essential Features

### Preprocessor Directives

### Object Files

An object file is a work product that is output from the compiler. The object file will depend on the platform for which the program is compiled. The platform dependencies will include the processor instruction set but there can then be other dependencies such as the available systems call to an underlying operating system.

![object-file-formats](https://github.com/HenrikSamuelsson/reading-extreme-c/assets/5353030/233eff56-d127-4ef7-8f49-3351de5533bd)

*Figure: Family three of some object file formats.*

The above figure shows the evolvement of objects file formats. First there was assembler output (a.out) which evolved into Common Object File Format (COFF). Then more recently there is Portable Execution (PE) for Windows, Mach-O for Apple OS/X, and Executable and Linkable Format (ELF) for Unix. Note that ELF is not limited to UNIX since it is cross platform and is for example commonly used in embedded systems.
