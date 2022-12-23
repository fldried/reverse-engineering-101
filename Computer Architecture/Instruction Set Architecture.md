# Instruction Set Architecture (ISA)
Instruction set architecture (ISA) is the set of instructions that a processor is capable of executing. It defines the operations that the processor can perform, the registers that it can use, and the format of the instructions.
At this point, you already know of the various types of instructions and have seen examples of them.
You also know about registers and how they are used to store data and instructions. The ISA defines the registers that are available and how they are used.
Therefore, we will only look at the format of the instructions in this section.

## Instruction Format
The instruction format defines the way that instructions are encoded and decoded by the processor. It specifies the size of the instructions, the number of operands that each instruction can have, and the way that the operands are specified.

There are different ways that instruction format can be implemented. Some common types of instruction formats are:

| Instruction Format | Description |
| --- | --- |
| Fixed-length | In this format, all instructions have the same length. This makes it easy for the processor to decode the instructions, but it may result in a larger instruction set if many different types of instructions are needed. |
| Variable-length | In this format, the length of the instructions varies depending on the number of operands and the complexity of the operation. This can result in a more compact instruction set, but it can be more complex for the processor to decode the instructions. |
| RISC | Reduced instruction set computer (RISC) is a type of instruction format that is designed to be simple and efficient. It is based on the idea that a small number of simple instructions can be used to perform complex operations. |
| CISC | Complex instruction set computer (CISC) is a type of instruction format that is designed to be flexible and powerful. It is based on the idea that a small number of simple instructions can be used to perform complex operations. |
| Register-based | In this format, the operands of an instruction are specified using registers. This can reduce the size of the instructions, but it may require more instructions to access memory locations. |
| Immediate | In this format, the operands of an instruction are embedded directly in the instruction. This can be convenient for operations that only use a small number of constants, but it may increase the size of the instruction set. |

## Links
### For a more in-depth look at Computer Architecture, check out the Deep Dive section of this topic.
- [Deep Dive](../Readme.md#deep-dive)
### Back to this topics Table of Contents
- [Computer Architecture](Readme.md)
### Back to the Reverse Engineering Guide's Table of Contents
- [Reverse Engineering](../Readme.md)