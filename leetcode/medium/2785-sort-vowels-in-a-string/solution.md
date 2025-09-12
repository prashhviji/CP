# 2785. Sort Vowels in a String

**Link:** https://leetcode.com/problems/sort-vowels-in-a-string/submissions/1767820436/

Given a 0-indexed string s, permute s to get a new string t such that: All consonants remain in their original places. More formally, if there is an index i with 0 <= i < s.length such that s[i] is a consonant, then t[i] = s[i]. The vowels must be sorted in the nondecreasing order of their ASCII values. More formally, for pairs of indices i, j with 0 <= i < j < s.length such that s[i] and s[j] are vowels, then t[i] must not have a higher ASCII value than t[j]. Return the resulting string. The vowels are 'a', 'e', 'i', 'o', and 'u', and they can appear in lowercase or uppercase. Consonants comprise all letters that are not vowels.

```java
         for(char c: s.toCharArray()){
            if(isVowel(c)){
                temp.add(c);
            }
         }

         Collections.sort(temp);

         StringBuilder ans = new StringBuilder();
         int j =0;

         for(int i =0; i<s.length(); i++){
            if(isVowel(s.charAt(i))){
                ans.append(temp.get(j));
                j++;
            }else{
                ans.append(s.charAt(i));
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-2 had an unclosed `for` loop and a missing `ans.append(s.charAt(i))` inside the `else` block. Attempts 3-4 had incorrect vowel checking (`== "a"` instead of `=='a'`). Attempt 6-7 missed incrementing `j` in the `else` block.

2. **Evolution**:  Attempts progressed from syntax errors (unclosed loops) to logic errors (incorrect vowel checking and conditional logic within the loop).  The vowel check was eventually corrected. The `else` block was not properly handled consistently across attempts.

