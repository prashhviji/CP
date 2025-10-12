# 3539. Find Sum of Array Product of Magical Sequences

**Link:** https://leetcode.com/problems/find-sum-of-array-product-of-magical-sequences/submissions/1799448788/

You are given two integers, m and k, and an integer array nums. A sequence of integers seq is called magical if: seq has a size of m. 0 <= seq[i] < nums.length The binary representation of 2seq[0] + 2seq[1] + ... + 2seq[m - 1] has k set bits. The array product of this sequence is defined as prod(seq) = (nums[seq[0]] * nums[seq[1]] * ... * nums[seq[m - 1]]). Return the sum of the array products for all valid magical sequences. Since the answer may be large, return it modulo 109 + 7. A set bit refers to a bit in the binary representation of a number that has a value of 1.

```java
            for (int cnt = 1; cnt <= m; cnt++) {
        for (int i = 0; i < n; i++) {
            pow[i][0] = 1;
        }

        int[][] pow = new int[n][m + 1];
                C[i][j] = (C[i-1][j-1] + C[i-1][j]) % MOD;
            }
            C[i][0] = C[i][i] = 1;
            for (int j = 1; j < i; j++) {
        int[][] C = new int[m + 1][m + 1];
        for (int i = 0; i <= m; i++) {
        int n = nums.length;

        int MOD = (int) (1e9 + 7);
    public int magicalSum(int m, int k, int[] nums) {
                pow[i][cnt] = (int)((long)pow[i][cnt-1] * nums[i] % MOD);
            }
```
