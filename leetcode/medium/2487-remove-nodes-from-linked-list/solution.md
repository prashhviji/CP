# 2487. Remove Nodes From Linked List

**Link:** https://leetcode.com/problems/remove-nodes-from-linked-list/submissions/1753346444/

You are given the head of a linked list. Remove every node which has a node with a greater value anywhere to the right side of it. Return the head of the modified linked list.

```java
    public ListNode removeNodes(ListNode head) {
        if(head == null){
            return null;
        }
        ListNode curr = head;
        ListNode greater = removeNodes(curr.next);

        curr.next = greater;

        if(greater == null || curr.val >= greater.val){
            return curr;
        }
    }
        return greater;
}
```

## Mistake Analysis

TAGS: Logic Error, Null Pointer, Conditional Logic

1. **Key Issues**: Attempts 1-4 all suffer from incorrect conditional logic within the recursive calls.  Attempt 1-3 has a missing `return` statement.  Null pointer exceptions could occur if `nxtGreater` or `greater` is null and its value is accessed without a check.

2. **Evolution**: Attempts progressed toward a correct conditional (`greater == null || curr.val >= greater.val`), but failed to address the missing return statement in attempts 1-3.  The logic for removing nodes based on right-side greater values is fundamentally flawed in all attempts; they don't correctly iterate and compare.

