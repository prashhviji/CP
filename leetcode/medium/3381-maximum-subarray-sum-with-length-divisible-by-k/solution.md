# 3381. Maximum Subarray Sum With Length Divisible by K

**Link:** https://leetcode.com/problems/maximum-subarray-sum-with-length-divisible-by-k/submissions/1840705849/

You are given an array of integers nums and an integer k. Return the maximum sum of a subarray of nums, such that the size of the subarray is divisible by k.

```java
        long prefixSum = 0;
        long maxSum = Long.MIN_VALUE;
        long[] kSum = new long[k];
        for (int i = 0; i < k; i++) {
            kSum[i] = Long.MAX_VALUE / 2;
        }
        kSum[k - 1] = 0;
        for (int i = 0; i < n; i++) {
            prefixSum += nums[i];
            maxSum = Math.max(maxSum, prefixSum - kSum[i % k]);
            kSum[i % k] = Math.min(kSum[i % k], prefixSum);
        }
        return maxSum;
    }
}
        int n = nums.length;
    public long maxSubarraySum(int[] nums, int k) {
```
