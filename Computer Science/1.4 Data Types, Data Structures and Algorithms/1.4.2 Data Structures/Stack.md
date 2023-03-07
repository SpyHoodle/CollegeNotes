# Stack
2022-11-29 | [1.4.2 Data Structures](1.4.2%20Data%20Structures.md)

- **Stack** -> A dynamic data structure that follows FILO (first in last out)
  - As data is placed in the stack, it cannot be accessed until the data that was more recently placed in the stack was removed
  - Therefore the first in data will be the last data to come out of the stack

## Methods
- You can only add or remove to the top of a stack
	- Methods of `push()` and `pop()`
- Methods to check whether the stack `is_empty()` or `is_full()`

## Attributes
- Size of the stack (length)
- **Stack pointer** -> Points to the position of where a new item will go when it is pushed onto the stack
	- The pointer always points to the top of the stack so it must be adjusted

## Implementation
- **Linked List**: Restrictions so that it can only push and pop from just the end (or the just the head)
- **Array**: Use an array and a variable and a couple of functions, just move the stack pointer every time items are pushed or popped
	- Prevent overflow, as the stack pointer may go out of the size of the box
