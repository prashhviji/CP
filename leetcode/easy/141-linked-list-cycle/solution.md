# 141. Linked List Cycle

**Link:** https://leetcode.com/problems/linked-list-cycle/submissions/1753305018/

Given head, the head of a linked list, determine if the linked list has a cycle in it. There is a cycle in a linked list if there is some node in the list that can be reached again by continuously following the next pointer. Internally, pos is used to denote the index of the node that tail's next pointer is connected to. Note that pos is not passed as a parameter. Return true if there is a cycle in the linked list. Otherwise, return false.

```java
        ListNode slow = head;

        while(fast!=null && fast.next!= null){
        ListNode fast = head;
            fast = fast.next.next;
            slow = slow.next;
    public boolean hasCycle(ListNode head) {
 */
public class Solution {
 *     }
 * }
 *         next = null;
            if(slow == fast){
            return true;
            }
        }
        return false;
        
```

## Mistake Analysis

TAGS: Loop Logic, Null Pointer, Logic Error

1. **Key Issues**: Attempts 1-3 had incorrect loop conditions or `NullPointerException` risks. Attempts 4-6 had syntax errors (missing brackets, misplaced code blocks) preventing compilation.  The core logic (fast/slow pointers) was flawed in early attempts.

2. **Evolution**:  Attempts progressed toward the correct `while` loop condition (`fast != null && fast.next != null`) to avoid `NullPointerException`.  However, syntax errors hindered success until Attempt 5 corrected the structural issues.  Attempt 6 is a variation of the final working solution.

