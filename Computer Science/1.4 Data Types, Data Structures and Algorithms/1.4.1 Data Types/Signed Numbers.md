# Signed Numbers
2022-09-29 | [1.4.1 Data Types](1.4.1%20Data%20Types.md)

## Sign and Magnitude
- **Sign** -> +/-
- **Magnitude** -> 255
- The most important bit becomes the sign
	- Most important bit means the one which will have the biggest effect if it's lost
	- 0 -> +
	- 1 -> -
- This does not work for calculations

## Two's Compliment
- Used for calculations
- The most important bit becomes negative
	- 128 -> -128
- $\text{2s compliment} = \text{1s compliment} + 1$
- To get a negative number -> flip all the bits, add one to the last digit
- To subtract two numbers, take the negative of one then add them together
