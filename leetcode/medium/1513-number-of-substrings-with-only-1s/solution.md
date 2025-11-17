# 1513. Number of Substrings With Only 1s

**Link:** https://leetcode.com/problems/number-of-substrings-with-only-1s/submissions/1832600079/

Given a binary string s, return the number of substrings with all characters 1's. Since the answer may be too large, return it modulo 109 + 7.

```java
    public int numSub(String s) {
        long cnt = 0, total = 0, mod = 1000000007;
        for (int i = 0; i < s.length(); i++) {
            if (s.charAt(i) == '1') {
                cnt++;
            } else {
                cnt = 0;
            }
            total = (total + cnt) % mod;
        }
        return (int) total;
    }
}
class Solution {
```
