# The Processor
2023-01-10 | [1.1.1 Structure and Function of The Processor](1.1.1%20Structure%20and%20Function%20of%20The%20Processor.md)


## Processor
- **CPU** -> responsible for executing the instructions of programs
- **ALU** -> responsible for performing arithmetic calculations and logical operations
	- Addition, subtraction, division, etc.
	- AND, OR, NOT, etc.
	- Comparisons between values, such as greater than, less than
	- Shifting binary patterns to the left or right
- **Control Unit** -> in charge of organising the sequence in which program instructions are executed, followed by decoding the instruction

## Clock
- **Clock** -> generates regular clock pulses by emitting a signal that continuously oscillates between a low (or '0') and a high (or '1') state
	- Used to synchronise the operations of the processor components
	- **Rising edge** -> change from 0 to 1
	- **Falling edge** -> change from 1 to 0
- **Clock period** -> time taken between two sequential rising edges (time taken for one **clock cycle**)
	- Every operation typically requires multiple clock cycles to complete, even if it is described as one operation (e.g. fetching data from memory)
	- The number of cycles is specific to each processor
- **Clock frequency** $\text{measured in Hz}$ -> calculated as the number of clock cycles that can be completed in one second
	- Inverse of the clock period, therefore: $\text{clock frequency} = \frac{1}{\text{clock period}}$
	- $1\text{Hz}$ is one cycle per second

## Registers
- **General-purpose registers** -> the ALU is connected to a set of general-purpose registers that are used to keep results of intermediate calculations to speed up execution
- **Program counter** (PC) -> holds the address of the next instruction to be executed by the processor
- **Current instruction register** (CIR) -> holds the current instruction that the processor is executing
- **Status register** (SR) -> used to store information about the result of the last instruction that the ALU executed
	- Each bit within the status register acts as a flag to indicate if an error or exception has occurred within the process, or to enable or disable interrupts to be raised
	- **Error or exception** -> when the result of a calculation requires further action
	- **Interrupt** -> an event outside of the program that requires the attention of the processor (e.g hardware malfunction)
- **Memory address register** (MAR) -> temporarily holds the address of the memory address (location in main memory) that the processor needs to access, either to read from (i.e. load data) or write (i.e. store data) to
- **Memory data register** (MBR/MDR) -> temporarily holds the data (data values or instructions) that are read from or written to the main memory
- **Accumulator** -> stores the result of any calculation processed by the ALU
	- The processor accesses other general-purpose registers where temporary values are stored while calculations are completed
	- Any result resides in the accumulator

## Fetch-Decode-Execute Cycle
#### Fetch
- The program counter (PC) keeps the address of the next instruction to be executed
- The contents of the PC are copied to the MAR which is connected to the address bus
- The address of the next instruction to be executed is placed on the address bus
- Once the address of the instruction is on the address bus, the control unit instructs a memory read operation to allow the contents of the memory location to be transferred to the processor
- The instruction that is stored at that address is transferred using the data bus from the main memory to the processor, and is saved in the memory MDR
- The contents of the MDR are copied to  the CIR.
- This ensures that the current instruction is kept safe so that the MDR can be used during the execute stage, in order to store additional data that is needed
#### Decode
- The control unit decodes the instruction that is kept in the CIR
- splitting the instruction into operand and opcode to determine what type of instruction needs to be carried out
- checking if additional data are required from memory
- figuring out where these are kept in main memory
#### Execute
- The instruction is executed
- The exact sequence of operations depends on the type of instruction that is being executed
- E.g, for an arithmetic instruction (such as adding two numbers together) any required data are fetched from the main memory, then the calculation is executed by the ALU, and the result of the instruction is stored in the accumulator, a general-purpose register, or back into main memory
