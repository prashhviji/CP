# 1930. Unique Length-3 Palindromic Subsequences

**Link:** https://leetcode.com/problems/unique-length-3-palindromic-subsequences/submissions/1836045633/

Given a string s, return the number of unique palindromes of length three that are a subsequence of s. Note that even if there are multiple ways to obtain the same subsequence, it is still only counted once. A palindrome is a string that reads the same forwards and backwards. A subsequence of a string is a new string generated from the original string with some characters (can be none) deleted without changing the relative order of the remaining characters.

```python
class Solution:
    def countPalindromicSubsequence(self, s: str) -> int:
        return sum([len(set(s[s.index(letter)+1:s.rindex(letter)])) for letter in set(s)])
```
