# 1015. Smallest Integer Divisible by K

**Link:** https://leetcode.com/problems/smallest-integer-divisible-by-k/submissions/1839477755/

Given a positive integer k, you need to find the length of the smallest positive integer n such that n is divisible by k, and n only contains the digit 1. Return the length of n. If there is no such n, return -1.

```java
class Solution {
    public int smallestRepunitDivByK(int K) {
        int remainder = 0;
        for (int length_N = 1; length_N <= K; length_N++) {
            remainder = (remainder * 10 + 1) % K;
            if (remainder == 0) {
                return length_N;
            }
        }
        return -1;
    }
}
```
