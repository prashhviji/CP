# 160. Intersection of Two Linked Lists

**Link:** https://leetcode.com/problems/intersection-of-two-linked-lists/submissions/1753244888/

Given the heads of two singly linked-lists headA and headB, return the node at which the two lists intersect. If the two linked lists have no intersection at all, return null.

```java
        ListNode pb = headB;

        while(pa!=pb){
            if(pa == null){
        ListNode pa  = headA;
                pa = headB;
            }else{
                pa = pa.next;
            }

            if(pb == null){
                pb = headA;
            }else{
                pb = pb.next;
            }
        }
        return pa;
    }
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Loop Logic

1. **Key Issues**: Attempt 1 & 2 have syntax errors (missing semicolons, misplaced code blocks). All attempts have logic errors in the `while` loop condition and pointer updates.  They don't correctly handle the two-pointer approach for intersection detection. Attempt 3 is closer but still has an incorrect return statement within the loop.

2. **Evolution**: Attempts show progress in fixing syntax errors, but the core logic of the two-pointer method remains flawed across all attempts.  The `if` conditions for null checks are not properly integrated with the pointer movement.

