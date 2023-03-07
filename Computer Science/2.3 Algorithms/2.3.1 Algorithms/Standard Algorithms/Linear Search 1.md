# Binary Search
2023-03-02 | [Standard Algorithms](Standard%20Alogrithms.md)

- Requires a sorted list
- Uses 3 pointers -> High, Middle, Low
- Middle is calculated by `(High + Low) DIV 2`
- Checks if the middle value is the target, 
	- if it's bigger then the high pointer becomes the middle pointer - 1
	- if it's smaller then the low pointer becomes the middle pointer + 1
- Then the middle pointer is recalculated
- This repeats until the middle value it checks is the target
- If the pointers overlap, after checking the middle value, then the item must not be in the list

## Example
- List = `[30, 41, 44, 56, 60, 90, 99]`
- Target = `20`

- For a binary search, the low pointer will start as 0 and the high pointer will start at 6 (length of the list.)
- The middle pointer will be (High + Low) DIV 2 = 6 DIV 2 = 3
- The item at index 3 = 56. 56 is compared against the target 20 and found it was bigger than 20 
	- So the high pointer becomes the value of the middle pointer - 1, so it becomes 2
- The middle pointer is recalculated through (High + Low) DIV 2 = 2 DIV 2 = 1
- The item at index 1 is 41. 41 is greater than the target 20
	- So the high pointer becomes the value of the middle pointer -1, so it becomes 0
- The middle pointer is recalculated through (High + Low) DIV 2 = 0 DIV 2 = 0
- The value at the middle pointer is 30 (index 0), which is greater than 20.
- The high pointer becomes the value of the middle pointer -1, so it becomes -1
- However since high pointer < low pointer, this should be impossible so the list must not contain the target value 20