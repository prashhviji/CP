# 33. Search in Rotated Sorted Array

**Link:** https://leetcode.com/problems/search-in-rotated-sorted-array/submissions/1776297327/

There is an integer array nums sorted in ascending order (with distinct values).

```java
    public int search(int[] nums, int target) {
        
        for(int i =0; i< nums.length; i++){
            if(nums[i] == target){
                return i;
            }
        }
        
        return -1;
    }
}
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 and 2 had logic errors: `isFound` was declared after its use, and the return statement `return i;` used an out-of-scope variable. Attempt 2 also incorrectly attempted to return `nums[i]` instead of the index `i`.

2. **Evolution**: The attempts progressed from a fundamentally flawed approach (incorrect placement of `isFound` and incorrect return values) to a correct linear search implementation in Attempt 3.  The final attempt correctly returns the index or -1 if not found.

