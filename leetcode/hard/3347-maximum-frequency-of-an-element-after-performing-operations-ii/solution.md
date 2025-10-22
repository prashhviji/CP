# 3347. Maximum Frequency of an Element After Performing Operations II

**Link:** https://leetcode.com/problems/maximum-frequency-of-an-element-after-performing-operations-ii/submissions/1808563700/

You are given an integer array nums and two integers k and numOperations. You must perform an operation numOperations times on nums, where in each operation you: Select an index i that was not selected in any previous operations. Add an integer in the range [-k, k] to nums[i]. Return the maximum possible frequency of any element in nums after performing the operations.

```java
        return l;
    }

    public int maxFrequency(int[] nums, int k, int numOperations) {
        int m = numOperations;
        Arrays.sort(nums);
        int ans = 1;
        for (int i = 0; i < nums.length - 1; i++) {
            ans = Math.max(ans, check(nums, nums[i], k, m));
            ans = Math.max(ans, check(nums, nums[i] - k, k, m));
            ans = Math.max(ans, check(nums, nums[i] + k, k, m));
        }
        return ans;
    }
}

```
