# 28. Find the Index of the First Occurrence in a String

**Link:** https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/submissions/1774729173/

Given two strings needle and haystack, return the index of the first occurrence of needle in haystack, or -1 if needle is not part of haystack.

```java
            for(int needleIndex = 0; needleIndex < needleLen ; needleIndex++){
                if(haystack.charAt(startIndex + needleIndex) != needle.charAt(needleIndex)){
                    isMatch = false;
                }
            }


            boolean isMatch = true;
        for(int startIndex = 0; startIndex <= haystackLen - needleLen; startIndex++){

        int needleLen = needle.length();
        int haystackLen = haystack.length();
        }
            return 0;
        if(needle.length() == 0){
    public int strStr(String haystack, String needle) {
class Solution {
```

## Mistake Analysis

TAGS: Loop Logic, Conditional Logic, Array Bounds

1. **Key Issues**: Attempt 1 lacks bounds checking for `haystack`. The inner loop assumes `haystack` is always longer than `needle` at every `startIndex`, leading to `ArrayIndexOutOfBoundsException`. The `isMatch` flag isn't reset for each `startIndex`.

2. **Evolution**: No subsequent attempts provided for analysis of improvement.

