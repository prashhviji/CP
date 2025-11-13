# 3228. Maximum Number of Operations to Move Ones to the End

**Link:** https://leetcode.com/problems/maximum-number-of-operations-to-move-ones-to-the-end/submissions/1828971637/

You are given a binary string s. You can perform the following operation on the string any number of times: Choose any index i from the string where i + 1 < s.length such that s[i] == '1' and s[i + 1] == '0'.

```java
        int ans = 0;
        int i = 0;
        while (i < s.length()) {
            if (s.charAt(i) == '0') {
                while (i + 1 < s.length() && s.charAt(i + 1) == '0') {
                    i++;
                }
                ans += countOne;
            } else {
                countOne++;
            }
            i++;
        }
    public int maxOperations(String s) {
        int countOne = 0;
public class Solution {

```
