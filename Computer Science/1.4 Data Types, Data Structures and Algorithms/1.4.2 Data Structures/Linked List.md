# Linked List
2022-11-22 | [1.4.2 Data Structures](1.4.2%20Data%20Structures.md)

- **Linked List** -> A dynamic abstract data structure where each element in the list points to the next
  - This means that data can be put anywhere and stored whilst keeping the order of the list as each element points to the next
- **Node** -> A single element in a linked list
	- A node is made up of two parts:
		- The data (which may be another complex data structure)
		- A pointer which is the index of the next node
	- It is possible to peek at nodes further forward in the linked list
- A start pointer identifies the first node in the list
- A next-free pointer shows the index of the next free space in the array

## Example
- Start points to the head of the list
- Each pointer field holds the index of the next node
- The last node has a null pointer
![2022-11-22-linked-list-diagram](2022-11-22-linked-list-diagram.png)

## Adding a node
- Put the data in the node pointed to by the next-free pointer
- Follow the pointers to find where the new node needs to be linked in
- Adjust the pointers
![2022-11-22-linked-list-diagram-adding-a-node](2022-11-22-linked-list-diagram-adding-a-node.png)

## Deleting a node
- To delete a node, we just need to adjust the pointers
- The deleted node can be linked back in to the list of free nodes by adjusting the pointer in the next-free and the pointer in the deleted node
![2022-11-22-linked-list-diagram-deleting-a-node](2022-11-22-linked-list-diagram-deleting-a-node.png)
