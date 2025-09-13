# 3541. Find Most Frequent Vowel and Consonant

**Link:** https://leetcode.com/problems/find-most-frequent-vowel-and-consonant/submissions/1769611531/

You are given a string s consisting of lowercase English letters ('a' to 'z'). Your task is to: Find the vowel (one of 'a', 'e', 'i', 'o', or 'u') with the maximum frequency. Find the consonant (all other letters excluding vowels) with the maximum frequency. Return the sum of the two frequencies.

```java
        int[] count = new int [26];
        int max_Vowel = 0, max_Consonant = 0;
        for(char c: s.toCharArray()){
            int i = c-'a';
            count[i]++;
            if (c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u')
                max_Vowel = Math.max(max_Vowel, count[i]);
            else
                max_Consonant = Math.max(max_Consonant, count[i]);
        }
        return max_Vowel + max_Consonant;
        
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic, Data Structure

1. **Key Issues**: Attempts 1-8 suffer from logic errors in updating `max_Vowel` and `max_Consonant`.  They inconsistently used `freq` and `count` arrays and didn't track the most frequent vowel/consonant correctly within the conditional statement. Attempt 9 fixed the array inconsistency but still needed method definition and return statement.


2. **Evolution**: Attempts iteratively corrected array naming inconsistencies.  A consistent approach to tracking maximum frequencies within the conditional logic was missing until the final attempt, which still lacks a complete code structure.

