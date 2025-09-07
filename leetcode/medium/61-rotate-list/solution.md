# 61. Rotate List

**Link:** https://leetcode.com/problems/rotate-list/

Given the head of a linked list, rotate the list to the right by k places.

```java
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next 
= next; }
 * }
 */
class Solution {
    public ListNode rotateRight(ListNode head, int k) {
       int length = 1;
       ListNode tail = head;
        while(tail.next != null){
            tail = tail.next;
            length++;
        }
        if(head == null || head.next == null) return head;
```

## Mistake Analysis

TAGS: Logic Error, Null Pointer, Loop Logic

1. **Key Issues**: Attempt 1 doesn't handle the empty list case (NullPointerException). The loop to find the tail is incorrect; it doesn't advance `length` if `head` is null.  The code is incomplete; it doesn't actually rotate the list.

2. **Evolution**: No further attempts were provided to analyze.

