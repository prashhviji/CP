# 3. Longest Substring Without Repeating Characters

**Link:** https://leetcode.com/problems/longest-substring-without-repeating-characters/submissions/1865146719/

Given a string s, find the length of the longest substring without duplicate characters.

```java
        int maxLength = 0;
        HashSet<Character> seen = new HashSet<>();

        while (right < s.length()) {
            char currentChar = s.charAt(right);
            if (!seen.contains(currentChar)) {
                seen.add(currentChar);
                maxLength = Math.max(maxLength, right - left + 1);
                right++;
            } else {
                seen.remove(s.charAt(left));
                left++;
            }
        }

        return maxLength;
    }
        int left = 0, right = 0;
    public int lengthOfLongestSubstring(String s) {
class Solution {

```
