# 876. Middle of the Linked List

**Link:** https://leetcode.com/problems/middle-of-the-linked-list/submissions/1749430816/

Given the head of a singly linked list, return the middle node of the linked list. If there are two middle nodes, return the second middle node.

```java
 */
class Solution {
    public ListNode middleNode(ListNode head) {
        ListNode fast = head;
        ListNode slow = head;

        while(fast!= null && fast.next!=null){
            slow = slow.next;
 * }
            fast = fast.next.next;
        }

        return slow;
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Null Pointer, Loop Logic

1. **Key Issues**: Attempts 1-4 had a missing `return slow;` statement, returning `slow.val` (an `int`) instead of `slow` (a `ListNode`).  Attempt 4 corrected the `->` operator to `.`.  Attempt 5 is incomplete.  Null pointer exceptions could occur if `fast.next` is checked before ensuring `fast` is not null.

2. **Evolution**: The code gradually corrected syntax (`->` to `.`) and the return type. The core logic using fast and slow pointers to find the middle node remained consistent, but the return statement was the major flaw across the attempts.

