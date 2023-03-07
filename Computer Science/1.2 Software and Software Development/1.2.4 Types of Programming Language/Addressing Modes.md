# Addressing Modes
2023-01-27 | [1.2.4 Types of Programming Language](1.2.4%20Types%20of%20Programming%20Language.md)

- **Addressing Modes** -> Specifies how the operand should be interpreted
	- They allow for a greater number of addresses to be accessed in main memory
	- Because the size of the operand would constrain the number of addresses that could be accessed
- Machine code -> `[OPCODE][ADDRESSING MODE][OPERAND]`

## Types
- **Immediate Addressing** -> The operand is the actual value
- **Direct Addressing** -> The operand gives an address which holds a value
- **Indirect Addressing** -> The operand gives an address of a register which holds another address, where the data is located
- **Indexed Addressing** -> The operand is added to the index register (but doesn't store the result in the index register), then data is retrieved from main memory at the address from the result
