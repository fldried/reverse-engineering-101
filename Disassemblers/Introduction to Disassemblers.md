# Introduction to Disassemblers

## What is a Disassembler?
A disassembler is a tool that translates machine code into human-readable assembly language. This is useful for reverse engineering because it allows us to understand the instructions that are being executed by a program.

## Why Use a Disassembler?
Disassemblers are useful for reverse engineering because they allow us to understand the instructions that are being executed by a program. This can be useful for understanding how a program works, identifying vulnerabilities, and identifying the functionality of a program.

## Disassembler Types
There are many different disassemblers available, each with their own strengths and weaknesses. Some disassemblers are designed for specific operating systems or architectures, while others are designed to be cross-platform and cross-architecture.

## Popular Disassemblers
### IDA Pro
IDA Pro is one of the most popular disassemblers available. IDA Pro is capable of disassembling a wide variety of file formats and architectures. Furthermore, IDA Pro supports python scripting which allows users to create custom plugins and scripts to extend the functionality of IDA Pro. IDA Pro is available for Windows, Linux, and macOS. IDA Pro is a commercial product and is not free.
### Ghidra
Ghidra is a free, open-source disassembler that is developed by the NSA. While some Disassemblers do not support assembly code patching straight out of the box, Ghidra does. Ghidra also ships with a Script Manager that allows users to create custom scripts to extend the functionality of Ghidra. Ghidra is available for Windows, Linux, and macOS.
### Radare2
Radare2 is a rewrite of radare. It is a free, open-source disassembler that is available for Windows, Linux, and macOS. Radare2 uses the iaito GUI by default, which is a Qt-based continuation of Cutter. R2 also supports plugins and scripting using the r2pipe API.
### Binary Ninja
Binary Ninja is another free, disassembler supporting python scripting and plugins. What makes Binary Ninja so special, is it's cloud-based analysis. This allows you to analyze binaries on the cloud, and then download the results to your local machine.
### OllyDbg
OllyDbg has been around for a long time, and is still used by many people. Unlike many other disassemblers, OllyDbg focusses primarily on dynamic analysis. OllyDbg is no longer being maintained. I decided to include it here, solely because some very popular Reverse Engineering courses still use it. (I'm looking at you, begin.re)
### x64dbg
Technically, x64dbg is a debugger, but it features a disassembler as well. x64dbg is built on many other open-source projects, such as ScyllaHide, Zydis, TitanEngine, and more.
x64dbg features a plugin system using C++. 

## Links
### Next Session
- [Using Disassemblers](Using%20Disassemblers.md)
### Back to this topics Table of Contents
- [Disassemblers](Table%20of%20Contents.md)
### Back to the Reverse Engineering Guide's Table of Contents
- [Reverse Engineering](../README.md)