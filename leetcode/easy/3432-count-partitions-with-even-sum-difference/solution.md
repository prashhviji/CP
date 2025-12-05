# 3432. Count Partitions with Even Sum Difference

**Link:** https://leetcode.com/problems/count-partitions-with-even-sum-difference/submissions/1847711803/

You are given an integer array nums of length n. A partition is defined as an index i where 0 <= i < n - 1, splitting the array into two non-empty subarrays such that: Left subarray contains indices [0, i]. Right subarray contains indices [i + 1, n - 1]. Return the number of partitions where the difference between the sum of the left and right subarrays is even.

```java
class Solution {

    public int countPartitions(int[] nums) {
        int totalSum = 0;
        for (int x : nums) {
            totalSum += x;
        }
        return totalSum % 2 == 0 ? nums.length - 1 : 0;
    }
}
```
