# 3370. Smallest Number With All Set Bits

**Link:** https://leetcode.com/problems/smallest-number-with-all-set-bits/submissions/1815159324/

You are given a positive number n. Return the smallest number x greater than or equal to n, such that the binary representation of x contains only set bits

```java
class Solution {
    public int smallestNumber(int n) {
        int x = 1;
        while (x < n){
            x = x * 2 + 1;
        }
        return x;
    }
}
```
