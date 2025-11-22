# 3190. Find Minimum Operations to Make All Elements Divisible by Three

**Link:** https://leetcode.com/problems/find-minimum-operations-to-make-all-elements-divisible-by-three/submissions/1836449826/

You are given an integer array nums. In one operation, you can add or subtract 1 from any element of nums. Return the minimum number of operations to make all elements of nums divisible by 3.

```java
            int rem = x % 3;
            sum += Math.min(rem, 3 - rem);
        }
        return sum;
    }
}
        for (int x : nums) {
        int sum = 0;
class Solution {

    public int minimumOperations(int[] nums) {
```
