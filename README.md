# Reading Extreme C

Material related to reading the book Extreme C, written by Kamran Amini (Packt Publishing October 2019).

## Object Files

An object file is a work product that is output from the compiler. The object file will depend on the platform for which the program is compiled. The platform dependencies will include the processor instruction set but there can then be other dependencies such as the available systems call to an underlying operating system.

![assembly-variants-black-white drawio](https://github.com/HenrikSamuelsson/reading-extreme-c/assets/5353030/ec52bb8f-8986-4544-b8b8-b68e80a934e5)

*Figure: Family three of some object file formats.*

The above figure shows the evolvement of objects files. First there was assembler output (a.out) which evolved into Common Object File Format (COFF). Then more recently there is Portable Execution (PE) for Windows, Mach-O for Apple OS/X, and Executable and Linkable Format (ELF) for Unix. Note that ELF is not limited to UNIX since it is cross platform and is for example commonly used in embedded systems.
