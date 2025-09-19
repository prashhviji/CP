# 704. Binary Search

**Link:** https://leetcode.com/problems/binary-search/submissions/1775960828/

Given an array of integers nums which is sorted in ascending order, and an integer target, write a function to search target in nums. If target exists, then return its index. Otherwise, return -1. You must write an algorithm with O(log n) runtime complexity.

```java
class Solution {
    public int search(int[] nums, int target) {
        boolean isFound = false;
        for(int i =0; i< nums.length; i++){
            if(nums[i] == target){
                isFound = true;
            }
        }
    }
                return i;
        return -1;

}
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Algorithm Choice

1. **Key Issues**: All attempts use linear search (O(n)), not binary search (O(log n)).  Attempts 1-3 have syntax errors: unreachable code and improper return statements. Attempt 4 returns `i` without checking `isFound`.

2. **Evolution**: Attempts progressively fixed syntax errors, moving towards a correct return value (-1).  However, none implemented the correct binary search algorithm.

