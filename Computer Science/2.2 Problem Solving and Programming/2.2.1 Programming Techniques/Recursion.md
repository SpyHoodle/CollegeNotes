# Recursion
2022-12-13 | [2.2.1 Programming Techniques](2.2.1%20Programming%20Techniques.md)

- **Recursion** -> The ability of a subroutine to call itself
	- Recursive functions have to stop calling themselves at some point or it will keep running until all the available memory is taken up causing a stack overflow
	- Splitting a problem into the smaller problems first, instead of splitting, doing, then splitting and doing again and again (iteration)
- **Stack Frame (Recursion)** -> A record that contains the value of any parameters and local variables and the position in the subroutine that was reached when another subroutine was called
- **Call stack** -> The stack of all the stack frames

## Advantages
- Easy to implement recursive functions in mathematics like factorial
	- As factorial $5! = 4! \times 5$ etc.
- Easier to read and understand by humans than non recursive solutions
- Makes natural sense for some problems e.g. Tower of Hanoi

## Disadvantages
- If used incorrectly can cause stack overflows
- Extremely difficult to debug and trace through
- Uses a lot of memory as the call stack is needed
- Slower because of the need to manage stack operations

