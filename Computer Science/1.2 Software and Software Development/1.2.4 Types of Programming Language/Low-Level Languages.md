# Low Level Languages
2023-01-24 | [1.2.4 Types of Programming Language](1.2.4%20Types%20of%20Programming%20Language.md)

## Machine Code
- **Machine Code** -> The binary code that the CPU executes
	- All other languages must be translated to this before execution
	- Hexadecimal is usually used to represent this
- **Opcode** -> The part of the instruction that specifies which operation the CPU should execute
- **Operand** -> Contains a value or set of values relevant to the opcode, it could be data or an address in memory

## Assembly
- **Assembly languages** -> Machine code is written using a set of mnemonics that represent the binary equivalent in machine code
- Needs to be converted into machine code for execution, called assembling, which is done by using a translator called an assembler
- They directly translate into machine code (1:1 relationship)

### Advantages
- Allows a programmer to write extremely optimised programs
- When a system has limited resources, low-level languages allow a programmer to directly control how resources are used

### Disadvantages
- More difficult to write programs as programmers need a very good understanding of the hardware
- Not portable as they are specific to a particular instruction set/CPU
- Do not have libraries of functions that can be imported, the programmer has to write every process required for a program themselves

### Uses
- Embedded systems as they are restricted in resources, and have to be extremely efficient at completing their tasks
- Device drivers as it allows the CPU to communicate with the peripheral directly
