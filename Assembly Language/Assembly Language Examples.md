# x86 Assembly Examples
Here is some examples including detailed explanations of syntax and concepts.

## Arithmetic Instructionsc
### Addition
```asm
; Add the values in EAX and EBX and store the result in EAX
add eax, ebx
```

### Subtraction
```asm
; Subtract the value in ECX from the value in EAX and store the result in EAX
sub eax, ecx
```

### Multiplication
```asm
; Multiply the value in EAX by the value in ECX and store the result in EAX
mul ecx
```
#### Note: We did not have to specify the destination register because the result is always stored in EAX.
#### Note: The value in EDX is also overwritten, because it is used to store the high-order bits of the result. If you need to preserve the value in EDX, you can use the `imul` instruction instead.

### Division
```asm
; Divide the value in EAX by the value in ECX and store the result in EAX
div ecx
```

## Logical Instructions
### AND
```asm
; Perform a bitwise AND of the values in EAX and EBX and store the result in EAX
and eax, ebx
```

### OR
```asm
; Perform a bitwise OR of the values in EAX and EBX and store the result in EAX
or eax, ebx
```

### XOR
```asm
; Perform a bitwise XOR of the values in EAX and EBX and store the result in EAX
xor eax, ebx
```

### NOT
```asm
; Perform a bitwise NOT of the value in EAX and store the result in EAX
not eax
```

## Data Transfer Instructions
Data transfer instructions move data between registers and memory locations.
```asm
; Move the value in EAX into the memory location pointed to by EBX
mov [ebx], eax

; Move the value at the memory location pointed to by EBX into EAX
mov eax, [ebx]

; Move the value 4 into the EAX register
mov eax, 4
```

## Control Flow Instructions
Control flow instructions change the flow of execution in a program, such as by jumping to a different location or calling a function.
```asm
; Jump to the label "loop"
jmp loop

; Call the printf function
call printf

; Return from the current function
ret
```

## Other Instructions
There are many other types of assembly language instructions, including stack manipulation instructions, interrupt instructions, and flag manipulation instructions. Here are a few examples of these instructions:
```asm
; Push the value in EAX onto the stack
push eax

; Pop the top value off the stack and store it in EAX
pop eax

; Execute an interrupt
int 0x80

; Set the zero flag if the result of the previous operation was zero
setz al

; Clear the carry flag
clc
```

### For more information on x86 instructions, see the following resource:
- [x86 Instructions](https://www.cs.virginia.edu/~evans/cs216/guides/x86.html#Instructions)

## Links
### Back to this topics Table of Contents
- [Assembly](Table%20of%20Contents.md)
### Back to the Reverse Engineering Guide's Table of Contents
- [Reverse Engineering](../README.md)
