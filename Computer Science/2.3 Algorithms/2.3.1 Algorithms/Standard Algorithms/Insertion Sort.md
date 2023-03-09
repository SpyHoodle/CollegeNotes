# Insertion Sort
2023-03-09 | [Standard Algorithms](Standard\ Algorithms.md)

## Double-Space Implementation
- Uses two lists, sorted and unsorted
- Each item is copied from the unsorted list and copied into the sorted list in the correct position
- Bad space complexity as you need another list the same size which means $O(n)$ 

## In-place Implementation
- The original list is used still
- Repeatedly swap the next element with the one to its left if smaller
- The temp value could be index 0 or the end of the list
- Good space complexity as you don't use anything but a temp space for all scenarios which means $O(1)$
