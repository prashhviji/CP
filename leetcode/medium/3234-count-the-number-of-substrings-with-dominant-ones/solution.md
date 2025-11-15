# 3234. Count the Number of Substrings With Dominant Ones

**Link:** https://leetcode.com/problems/count-the-number-of-substrings-with-dominant-ones/submissions/1830332861/

You are given a binary string s. Return the number of substrings with dominant ones. A string has dominant ones if the number of ones in the string is greater than or equal to the square of the number of zeros in the string.

```java
            int j = i;
            int cnt0 = s.charAt(i - 1) == '0' ? 1 : 0;
        int res = 0;
        for (int i = 1; i <= n; i++) {
        }
            }
                pre[i + 1] = pre[i];
            } else {
                pre[i + 1] = i;
            if (i == 0 || (i > 0 && s.charAt(i - 1) == '0')) {
        int[] pre = new int[n + 1];
        pre[0] = -1;
        for (int i = 0; i < n; i++) {

    public int numberOfSubstrings(String s) {
        int n = s.length();
class Solution {
```
