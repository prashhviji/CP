# 142. Linked List Cycle II

**Link:** https://leetcode.com/problems/linked-list-cycle-ii/submissions/1761905258/

Given the head of a linked list, return the node where the cycle begins. If there is no cycle, return null. There is a cycle in a linked list if there is some node in the list that can be reached again by continuously following the next pointer. Internally, pos is used to denote the index of the node that tail's next pointer is connected to (0-indexed). It is -1 if there is no cycle. Note that pos is not passed as a parameter. Do not modify the linked list.

```java
            slow = slow.next;
            if(slow == fast){
            fast = fast.next.next;
        while(fast!=null && fast.next!=null){

        ListNode fast = head;
        ListNode slow = head;
        if (head == null || head.next == null) return null;
    public ListNode detectCycle(ListNode head) {
public class Solution {
 */
 * }
 *     }
 *         next = null;
 *         val = x;
 *     ListNode(int x) {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Null Pointer

1. **Key Issues**: Attempts 1 & 2 incorrectly return `true`/`false` instead of the node.  Attempts 3-5 have incorrect loop structures and missing `ListNode` declaration,  leading to compile errors or incorrect results. Attempt 6 fixes return type but still needs proper loop nesting to find the cycle start.

2. **Evolution**: Attempts show progress towards the correct algorithm (Floyd's cycle detection).  The logic for finding the cycle's starting point was gradually refined, but syntactical issues and a flawed return type hindered the solution.  Attempt 6 finally correctly identifies the cycle start node, but the code is still badly formatted.

