# 206. Reverse Linked List

**Link:** https://leetcode.com/problems/reverse-linked-list/submissions/1866094419/

Given the head of a singly linked list, reverse the list, and return the reversed list.

```java
 */
class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode prev = null;
        ListNode current = head;

        while(current!=null){
            ListNode nextNode = current.next;
            current.next = prev;
            prev = current;
            current = nextNode;
        }
        return prev;
    }
}
```
