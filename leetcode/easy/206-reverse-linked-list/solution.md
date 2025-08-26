# 206. Reverse Linked List

**Link:** https://leetcode.com/problems/reverse-linked-list/submissions/1749406954/

Given the head of a singly linked list, reverse the list, and return the reversed list.

```java
 * }
 */
class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode prev = null;
        ListNode current = head;

        while(current!=null){
            ListNode nextNode = current.next;
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 *     ListNode() {}
 * public class ListNode {
 *     int val;
 *     ListNode next;
 * Definition for singly-linked list.
/**
            current.next = prev;
```

## Mistake Analysis

TAGS: Loop Logic, Logic Error, Null Pointer

1. **Key Issues**: Attempt 1 has a misplaced closing curly brace, causing a syntax error. The core loop logic is incomplete; it doesn't update `current` in each iteration, leading to an infinite loop if `current` is not null.  There's also potential for a NullPointerException if `head` is null.

2. **Evolution**: No subsequent attempts were provided to analyze improvement.

