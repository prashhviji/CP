# 3397. Maximum Number of Distinct Elements After Operations

**Link:** https://leetcode.com/problems/maximum-number-of-distinct-elements-after-operations/submissions/1805109208/

You are given an integer array nums and an integer k. You are allowed to perform the following operation on each element of the array at most once: Add an integer in the range [-k, k] to the element. Return the maximum possible number of distinct elements in nums after performing the operations.

```java
        Arrays.sort(nums);
        int ans = 0, prev = (int)-1e9;

        for (int x : nums) {
            int l = Math.max(x - k, prev + 1);
            if (l <= x + k) {
                prev = l;
                ans++;
            }
        }
        return ans;
    }
}
```
