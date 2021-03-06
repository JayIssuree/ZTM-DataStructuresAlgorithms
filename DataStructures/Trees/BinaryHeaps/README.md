# Binary Heaps
- Similar to a binary tree
- Every parent node an have 2 children nodes

- MAX HEAP => each CHILD NODE must be LESS THAN the PARENT NODE
    - It starts with the maximum value
- MIN HEAP => each CHILD NODE must be GREATER THAN the PARENT NODE
    - It starts with the minimum value

=> The root node will either be the largest/smallest element
- There is no relationship between left and right
- The only relationship is between top to bottom

- You can store a priority queue in an array
    - Each parents child will be stored at:
        LEFT: 2n + 1 
        RIGHT: 2n + 2
    - To find the parent of an element:
        (n - 1)/2.floor
    => Where n is the index in the array

- Commonly used in PRIORITY QUEUES
- Can be used in any algorithm where ORDERING is important
- Good at doing comparative operations => all values GREATER/LESS THAN X
- Take up the least amount of space
- There is no balancing needed like in a binary search tree
- It is balanced from left to right
- Higher valued insertions 'bubble up'

- Lookup => O(n)
- Insert => O(log n)
- Delete => O(log n)

# Priority Queue
- Similar to queues except the queue is based on priority
- Like an emergency room => there is a queue but the most severe injurues (highest value/priority) are treated first => high priorities bubble up to be treated first when inserted