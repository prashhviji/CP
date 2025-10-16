# 2598. Smallest Missing Non-negative Integer After Operations

**Link:** https://leetcode.com/problems/smallest-missing-non-negative-integer-after-operations/submissions/1803626908/

You are given a 0-indexed integer array nums and an integer value. In one operation, you can add or subtract value from any element of nums.

```java
class Solution {

    public int findSmallestInteger(int[] nums, int value) {
        int[] mp = new int[value];
        for (int x : nums) {
            int v = ((x % value) + value) % value;
            mp[v]++;
        }
        int mex = 0;
        while (mp[mex % value] > 0) {
            mp[mex % value]--;
            mex++;
        }
        return mex;
    }
}
```
