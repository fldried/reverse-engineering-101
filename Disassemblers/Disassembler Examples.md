# Disassembly Examples

Previously, we discussed some of the features that can be found in disassemblers. We also learned about the more popular disassemblers.
In this section, we will take a look at some examples of disassemblers in action.

To make things easier to understand, we will be using the same program for all of the examples. The program is a simple "Hello World" program written in C. The source code for the program is shown below:

```c
#include <stdio.h>

int main()
{
    printf("Hello World!\n");
    return 0;
}
```

The program is compiled using the following command:

```bash
gcc -o hello_world hello_world.c
```

We can now use a disassembler to disassemble the program. We will be using IDA Pro for all of the examples. The disassembly of the program is shown below:
![](https://i.imgur.com/J4DGe3h.png)

As you can see, the disassembly is very similar to the source code. The only difference is that the disassembly is in assembly language, and the source code is in C. This makes it much easier to understand what the program is doing.

## Analyzing the Disassembly

Now that we have the disassembly, we can start analyzing it. The first thing we can do is look at the main function. The main function is the entry point of the program. This is the function that is called when the program is executed.

The next thing we can do is look at the printf function. The printf function is used to print a string to the console. The string that is printed is the string that is passed to the function. In this case, the string that is passed to the function is "Hello World!\n".

![](https://i.imgur.com/TkjEWqc.png)

In case you're following along, you may have noticed the string "Hello World!\n" is not in the disassembly itself, but is added as a comment. This is because the string is stored in the data section of the program. The data section is not executed by the program. It is only used to store data that is used by the program.
There may be some differences to what you see in the disassembly, depending on the disassembler that you are using. However, the general idea is the same.

## Links
### Back to this topic's Table of Contents
- [Disassemblers](Table%20of%20Contents.md)
### Back to the Reverse Engineering Guide's Table of Contents
- [Reverse Engineering](../README.md)