# x86 Assembly Syntax

In this section, we will learn about the syntax of x86 assembly language. We will start by looking at the basic structure of an instruction, then we will look at the different types of operands that can be used in an instruction.

In x86 assembly language, each instruction is made up of a mnemonic (a short, human-readable name) and one or more operands (values or memory locations that the instruction operates on). The syntax for an x86 instruction is generally of the form:

```asm
mnemonic destination, source
```
where `destination` is the location where the result of the instruction will be stored and `source` is the location of the data that the instruction operates on.

## Example
```asm
mov eax, 0x12345678 ; move the value 0x12345678 into the EAX register
```

We will now take a quick glance at the different registers that are available in x86 assembly language.

## Registers
x86 processors have a number of registers that can be used to store values (data or addesses) and perform operations. The most common registers are:

| Register | Purpose | Explanation |
| -------- | ------- | ----------- |
| EAX | Accumulator register | The EAX register is used to store the result of arithmetic and logical operations. It is also used as a general-purpose register. |
| EBX | Base register | The EBX register is used as a general-purpose register. |
| ECX | Counter register | The ECX register is used as a counter for loop instructions. |
| EDX | Data register | The EDX register is used to store the result of multiplication and division operations. It is also used as a general-purpose register. |

There are also a number of other registers that are used for different purposes. For example, the ESP register is used to store the stack pointer, and the EIP register is used to store the instruction pointer, more on these later.

## Memory
In addition to registers, x86 assembly language allows you to access memory locations using a variety of addressing modes. For example, you can use the `[address]` syntax to access the value at a specific memory address, or you can use the `[base + index*scale + displacement]` syntax to access a value at an address that is calculated from a base address, an index value, and a displacement value. This is known as indirect addressing, and it is used to access data that is not stored in a register.

## Labels
Assembly language uses symbolic labels to represent memory locations. These labels can be used in place of absolute memory addresses, which makes the code easier to read and maintain. Labels are defined by a name followed by a colon (`:`), and they can be used in instructions by preceding them with a `jmp` or `call` instruction.

## Comments
x86 assembly language supports comments, which are used to add notes and documentation to your code. Comments start with a semicolon (`;`) and continue until the end of the line.

## Data Types
x86 assembly language supports a variety of data types, including integers, floating-point numbers, and strings. The size of these data types is determined by the number of bits they occupy in memory. For example, a `byte` is an 8-bit value, a `word` is a 16-bit value, and a `dword` is a 32-bit value.

## Instructions
x86 has a large number of instructions that can be used to perform a wide variety of tasks. Some common types of instructions include:

- Arithmetic instructions: These instructions perform basic arithmetic operations, such as addition, subtraction, multiplication, and division.
- Logical instructions: These instructions perform logical operations, such as AND, OR, XOR, and NOT.
- Data transfer instructions: These instructions move data between registers and memory locations.
- Control flow instructions: These instructions change the flow of execution in a program, such as by jumping to a different location or calling a function.

## Directives
In addition to instructions, x86 assembly language also features a number of directives that are used to provide information to the assembler. Some common directives include:
- `.data`: This directive is used to define data that will be stored in memory.	
- `.code`: This directive is used to define code that will be assembled into machine code.
- `.equ`: This directive is used to define a symbolic constant and symbolic value.

## Macros
x86 assembly language supports macros, which are reusable blocks of code that can be expanded by the assembler. Macros can be defined using the `%macro` and `%endmacro` directives, and they can be invoked using their name followed by a set of parameters. Macros can be used to simplify complex code and improve readability.

## Assemblers
To translate x86 assembly language into machine code, you will need to use an assembler. An assembler is a program that converts assembly language instructions into machine code that can be executed by the processor. There are many different assemblers available for x86, each with its own syntax and features.

## Linking
After assembling an x86 program, you will typically need to link it with other object files and libraries to create a complete executable. Linking combines the machine code from multiple sources into a single file and resolves any external references. There are many different linkers available for x86, each with its own syntax and features.

## Links
### Continue to Next Section
- [Assembly Language Examples](Assembly%20Language%20Examples.md)
### Back to this topics Table of Contents
- [Assembly](Table%20of%20Contents.md)
### Back to the Reverse Engineering Guide's Table of Contents
- [Reverse Engineering](../README.md)
