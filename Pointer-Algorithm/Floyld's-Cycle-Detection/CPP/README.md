Floyd's cycle finding algorithm, also known as the Hare-Tortoise algorithm is a pointer algorithm that traverses the sequence using two pointers moving at two distinct speeds. The loop in a linked list can be found using this approach. It employs two pointers, one of which moves twice the speed as the other. 
The two pointers are such that:
  1. The pointer which traverses two nodes at a time is called the fast pointer.
  2. The pointer which traverses one node at a time is called the slow pointer.
  
While traversing the two possibilities that can occur are:
  1. The fast pointer reaches NULL which implies that there is no loop present.
  2. The two pointers meet at a single node which implies that a loop is present.
  
Time Complexity: 0(n)
Space Complexity: 0(1)

This algorithm can further be used in finding the beginning node of the loop
Step 1: Following the algo we reach a point where both fast and slow node point a the same node (not the beginning node).
Step 2: Without making any change to the fast pointer, take the slow pointer to the head
Step 3: Now let both the pointer move with equal steps.
Step 4: The node where bothe the pointers meet is the required node.
