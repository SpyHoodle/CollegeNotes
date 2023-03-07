# Errors and Debugging
2022-01-02 | [2.2.1 Programming Techniques](2.2.1%20Programming%20Techniques.md)

## Types of Error
- **Syntax Error** -> Errors caused by not following the rules of the language
	- Common causes include:
		- Spelling errors
		- Missing brackets
- **Logic Error** -> Errors that cause a program to work unexpectedly
	- The computer runs the code perfectly fine but you have programmed it to do something that you weren't expecting
- **Semantic Error** -> Improper use of a program code statement, flagged by the compiler or translator
	- e.g. adding two undefined variables together
- **Runtime Error** -> Code is valid according to syntax and semantics, but the environment that the program is being run in causes an error
	- Inputs at runtime can cause errors
	- Can be prevented through try except blocks in python or general validation -> creating a more robust program
	- E.g. You try to convert a string to an integer from an input() statement in python where the user has entered alphabetical characters

## Rubber Duck Debugging
- Explain to the duck your program and what your error is
- Eventually you will realise what the issue is properly and understand how to solve it
- You may realise that you are not actually doing what you are supposed to be doing in the code