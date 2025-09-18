# 242. Valid Anagram

**Link:** https://leetcode.com/problems/valid-anagram/submissions/1774747327/

Given two strings s and t, return true if t is an anagram of s, and false otherwise.

```java
            return false;
        }

        char[] sArray = s.toCharArray();
        char[] tArray = t.toCharArray();

        Arrays.sort(sArray);
        Arrays.sort(tArray);

        return Arrays.equals(sArray, tArray);
    }
}

        if (s.length() != t.length()) {
    public boolean isAnagram(String s, String t) {
class Solution {
```
