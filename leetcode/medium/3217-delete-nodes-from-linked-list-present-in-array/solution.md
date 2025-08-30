# 3217. Delete Nodes From Linked List Present in Array

**Link:** https://leetcode.com/problems/delete-nodes-from-linked-list-present-in-array/submissions/1753349682/

You are given an array of integers nums and the head of a linked list. Return the head of the modified linked list after removing all nodes from the linked list that have a value that exists in nums.

```java
        ListNode temp = new ListNode();
        ListNode current = temp;

        while(head != null){
            if( head.val >= freq.length || freq[head.val] == false){
                current.next = head;
                current = current.next;
            }
            head = head.next;
        }

        current.next = null;
        return temp.next;
    }
}

        for(int num : nums) freq[num] = true;
```
