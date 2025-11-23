# 1262. Greatest Sum Divisible by Three

**Link:** https://leetcode.com/problems/greatest-sum-divisible-by-three/submissions/1837400868/

Given an integer array nums, return the maximum possible sum of elements of the array such that it is divisible by three.

```java
    public int maxSumDivThree(int[] nums) {
        int[] f = { 0, Integer.MIN_VALUE, Integer.MIN_VALUE };
        for (int num : nums) {
            int[] g = new int[3];
            System.arraycopy(f, 0, g, 0, 3);
            for (int i = 0; i < 3; ++i) {
                g[(i + (num % 3)) % 3] = Math.max(
                    g[(i + (num % 3)) % 3],
                    f[i] + num
                );
            }
            f = g;
        }
        return f[0];
    }

class Solution {
```
