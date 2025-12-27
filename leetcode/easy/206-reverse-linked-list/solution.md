# 206. Reverse Linked List

**Link:** https://leetcode.com/problems/reverse-linked-list/submissions/1866347313/

Given the head of a singly linked list, reverse the list, and return the reversed list.

```java
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode prev = null;
 * public class ListNode {
 *     int val;
 *     ListNode next;
        ListNode current = head;
        while(current != null){
            ListNode next = current.next;
        }
            current.next = prev;
            prev = current;
            current = next;
    }
        return prev;
```
