# 2487. Remove Nodes From Linked List

**Link:** https://leetcode.com/problems/remove-nodes-from-linked-list/submissions/1753346874/

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
class Solution {
```
