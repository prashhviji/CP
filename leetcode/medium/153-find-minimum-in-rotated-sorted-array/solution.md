# 153. Find Minimum in Rotated Sorted Array

**Link:** https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/submissions/1776277464/

```java
        int right = nums.length - 1;

        while (left < right) {
            int mid = left + (right - left) / 2;

            if (nums[mid] <= nums[right]) {
                right = mid;
            } else {
                left = mid + 1;
            }
        }

        return nums[left];        
    }
        int left = 0;
    public int findMin(int[] nums) {
class Solution {
```

## Mistake Analysis

TAGS: Loop Logic, Off By One, Algorithm Choice

1. **Key Issues**: Attempt 1 correctly implements binary search to find the minimum in a rotated sorted array. Attempt 2 has a misplaced `left` variable declaration and omits `left = 0` inside the function, resulting in a compilation error and incorrect logic. The `mid` calculation in Attempt 2 is also flawed.

2. **Evolution**: Attempt 1 is a functional solution. Attempt 2 introduces syntax errors that break the code's functionality.  The logic is improved in Attempt 1 by using `left + (right - left) / 2` to prevent integer overflow in `mid` calculation.

