# 540. Single Element in a Sorted Array

**Link:** https://leetcode.com/problems/single-element-in-a-sorted-array/submissions/1776292519/

You are given a sorted array consisting of only integers where every element appears exactly twice, except for one element which appears exactly once. Return the single element that appears only once. Your solution must run in O(log n) time and O(1) space.

```java
            if (mid % 2 == 1) mid--;

            if (nums[mid] == nums[mid + 1]) {
                left = mid + 2;
            } else {
                right = mid;
            }
        }

        return nums[left];

            int mid = left + (right - left) / 2;
        while (left < right) {

    }
        int left = 0, right = nums.length - 1;
    public int singleNonDuplicate(int[] nums) {
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-5 had uninitialized variables, incorrect loop logic, and faulty conditional statements for finding the single element. Attempt 6 partially worked but lacked handling of edge cases (single-element array). Attempt 7 correctly handled edge cases but used a linear scan instead of O(log n) algorithm.

2. **Evolution**: Attempts progressed from completely broken code to a linear-time solution (attempt 7). The attempts demonstrate improvement in conditional logic and handling edge cases, but fail to achieve the required logarithmic time complexity.

