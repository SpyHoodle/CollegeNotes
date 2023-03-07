# Complexity of Algorithms
2023-02-14 | [2.3.1 Algorithms](2.3.1%20Algorithms.md)

## Comparing Algorithms
- **Time complexity** -> Shows how the number of steps, time or space *changes* when input data *changes*
- **Big O Notation** -> Used to express the time complexity of performance of an algorithm
	- We use this as time is a poor indicator of performance as different machines may get different results
	- This can be done by measuring the number of steps
- Can be used for showing *time complexity* or *space complexity*
- Space complexity is dependent on the input data, but we don't account for the input data, i.e. it's how mu

### The Notation
- $O(1)$ -> Constant time complexity
	- Takes the same amount of time to execute no matter the size of the data set
	- E.g. `length = len(a)`
- $O(\log_{a} n)$ -> Logarithmic time complexity
	- E.g. Binary search -> $O(\log_{2} n)$
	- Doubling the size of the data set has very little effect on the time
- $O(n)$ -> Linear time complexity
	- Performance will grow in linear time, in direct proportion to the data set
- $O(n^a)$ -> Polynomial time complexity
	- Performance is directly proportional to the power $a$ of the size of the data set
- $O(a^n)$ -> Exponential time complexity
	- Time taken to execute will double with every additional item added to the data set
	- Quickly becomes very large
- $O(n!)$ -> Factorial time complexity

- Only the significant term is the one that is expressed
	- E.g. $O(2n + n^2) = O(n^2)$

![Time Complexity Graphs](../../../../Assets/2023-02-14-big-o-graphs.png)

### Calculating Time Complexity
- We need to count the number of basic operations it performs
- Nested loops are time complexity $O(n^a)$ where $a$ is the number of loops nested in each other
- Remember only the significant term is the one that is expressed

#### Example
```pseudocode
FOR k=1 to n-1
	isMinimum = True
	FOR j = 1 to n-1
		IF arrayX[k] > arrayX[j] THEN
			isMinimum = False
		ENDIF
	NEXT j
	IF (isMiniumum) THEN
		minimum = arrayX[k]
	ENDIF
NEXT k
```
- There are two basic operations in the main outer loop, (`isMinimum = true` and the final `IF` statement) which are each performed $n$ times. 
- The inner loop has one basic operations performed $n^2$ times.  
- This gives us a time complexity of $O(2n + n^2)$
- However only the significant term is expressed as time complexity, therefore the time complexity is only $O(n^2)$

## Types of Time Complexity
### Worst-case
- A good way to compare two algorithms is by looking at the worst-case time complexity
- E.g. in a linear search where the value to be found is at the end of the data, so the worst-case time complexity is $O(n)$

### Average and Best-Case
- When two algorithms have the same worst-case time complexity, it is useful to look at other types of complexities
- **Average time complexity** -> Based on the mean of the computational time required if you tried all the possible inputs in the system
	- e.g. in a linear search this would be about the middle of the data
- **Best-case time complexity** -> The most favourable scenario where the algorithm is fastest
	- e.g. in a linear search this would the start of the data