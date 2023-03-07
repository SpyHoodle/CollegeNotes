# Graph
2022-12-08 | [1.4.2 Data Structures](1.4.2%20Data%20Structures.md)

- **Graph** -> A data structure which has nodes which can be connected to multiple node and therefore does not have one singular linear order
	- **Edge** -> The 'connection' between multiple nodes (i.e. the line from one node to another)
	- **Weight** -> How difficult it would be to travel along a specific edge
	- **Neighbour** -> Two nodes connected by an edge
	- **Degree** -> Number of neigbours a node has
	- **Loop** -> A node with a connection to itself
	- **Cycle** -> A trail that starts and ends at the same node and no other node is visited more than once

## Representation
- **Adjacency Matrix** -> Mathematical representation -> Shows all the possible combinations
- **Adjacency List** -> Can be represented as a dictionary

## Types
- **Directed** -> Edges have a direction, you can only travel one way down an edge
- **Undirected** -> Edges don't have a direction, you can travel both ways along an edge
- **Weighted** -> Each edge has a weight, defining how difficult it would be to travel along it (i.e displacement between two nodes, time between two nodes)
