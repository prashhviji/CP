# 3461. Check If Digits Are Equal in String After Operations I

**Link:** https://leetcode.com/problems/check-if-digits-are-equal-in-string-after-operations-i/submissions/1809135811/

You are given a string s consisting of digits. Perform the following operation repeatedly until the string has exactly two digits: For each pair of consecutive digits in s, starting from the first digit, calculate a new digit as the sum of the two digits modulo 10. Replace s with the sequence of newly calculated digits, maintaining the order in which they are computed. Return true if the final two digits in s are the same; otherwise, return false.

```java
    public boolean hasSameDigits(String s) {
        int n = s.length();
        char[] sArray = s.toCharArray();
        for (int i = 1; i <= n - 2; i++) {
            for (int j = 0; j <= n - 1 - i; j++) {
                int digit1 = sArray[j] - '0';
                int digit2 = sArray[j + 1] - '0';
                sArray[j] = (char) (((digit1 + digit2) % 10) + '0');
            }
        }
        return sArray[0] == sArray[1];
    }
}
public class Solution {

```
