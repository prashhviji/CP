# 234. Palindrome Linked List

**Link:** https://leetcode.com/problems/palindrome-linked-list/submissions/1761892938/

Given the head of a singly linked list, return true if it is a palindrome or false otherwise.

```java
        int left =0;
        int right = arr.size()-1;
        while(left < right){
            if(!arr.get(left).equals(arr.get(right))){
                return false;
            }

            left++;
            right--;
        }
        return true;
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Space Complexity

1. **Key Issues**: Attempt 1 uses extra O(n) space to store the list in an ArrayList before checking for palindrome.  It's also incomplete; the palindrome check is unfinished.

2. **Evolution**: No further attempts were provided, preventing analysis of improvements.  A better approach would involve a two-pointer (slow/fast) technique to reverse the second half of the list in-place, reducing space complexity to O(1).

