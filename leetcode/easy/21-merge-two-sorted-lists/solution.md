# 21. Merge Two Sorted Lists

**Link:** https://leetcode.com/problems/merge-two-sorted-lists/submissions/1749450282/

You are given the heads of two sorted linked lists list1 and list2. Merge the two lists into one sorted list. The list should be made by splicing together the nodes of the first two lists. Return the head of the merged linked list.

```java
            list1.next=mergeTwoLists(list1.next,list2);
            return list1;

        if(list1!=null && list2!=null){
        if(list1.val<list2.val){
class Solution {
    public ListNode mergeTwoLists(ListNode list1, ListNode list2) {
 */
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 *     ListNode(int val) { this.val = val; }
 *     ListNode() {}
            }
            else{
                list2.next=mergeTwoLists(list1,list2.next);
                return list2;
        }
        }
```

## Mistake Analysis

TAGS: Syntax Error, Logic Error, Null Pointer

1. **Key Issues**: Attempt 1 has syntax errors (missing closing curly braces for the `if` and `else` blocks and the function), and a logic error in not handling the case when one list is null before the comparison.  A NullPointerException may occur if `list1.val` or `list2.val` is accessed when `list1` or `list2` is null.

2. **Evolution**: No further attempts provided to analyze improvement.

