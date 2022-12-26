# Parsing File Formats
This module will cover how to parse file formats. We will look at how to parse file formats using a variety of tools and techniques, including file signature analysis, file header analysis, and file format documentation.

## File Signature Analysis
File signature analysis is a technique used to identify the file format of a file. File signatures are a sequence of bytes that are used to identify the file format of a file. File signatures are usually stored at the beginning of a file and can be used to identify the file format of a file without having to parse the entire file.

On Windows systems, the `file` command can be used to identify the file format of a file using its file signature. For example, the `file` command can be used to identify the file format of a file named `test.exe` as follows:

```bash
$ file test.exe
> test.exe: PE32 executable (console) Intel 80386, for MS Windows
```

Here, the `file` command identified the file format of `test.exe` as a PE32 executable.
Looking at the file signature of `test.exe` in a hex editor, we can see that the file signature is `4D 5A`:

```bash
$ xxd test.exe
> 00000000: 4d5a 9000 0300 0000 0400 0000 ffff 0000  MZ..............
```

## File Header Analysis
File header analysis is a technique used to identify the file format of a file. File headers are a sequence of bytes that are used to identify the file format of a file. File headers are usually stored at the beginning of a file and can be used to identify the file format of a file without having to parse the entire file.

To parse a file format using file header analysis, the file header of the file format must be known. 
Here is a list of some common file headers:

| File Format | File Header |
| ----------- | ----------- |
| PE32 Executable | 4D 5A |
| PE32+ Executable | 4D 5A |
| ELF Executable | 7F 45 4C 46 |
| MACH-O Executable | CF FA ED FE |

## File Format Documentation
File format documentation is a technique used to identify the file format of a file. File format documentation is a set of instructions that describe the structure of a file format. File format documentation can be used to identify the file format of a file without having to parse the entire file.

To parse a file format using file format documentation, the file format documentation for the file format must be known. 
Here is a list of some common file format documentation:

| File Format | File Format Documentation |
| ----------- | ------------------------ |
| PE32 Executable | https://docs.microsoft.com/en-us/windows/win32/debug/pe-format |
| PE32+ Executable | https://docs.microsoft.com/en-us/windows/win32/debug/pe-format |
| ELF Executable | https://en.wikipedia.org/wiki/Executable_and_Linkable_Format |
| MACH-O Executable | https://en.wikipedia.org/wiki/Mach-O |

## Links
### Back to this topics Table of Contents
- [File Formats](Table%20of%20Contents.md)
### Back to the Reverse Engineering Guide's Table of Contents
- [Reverse Engineering](../README.md)