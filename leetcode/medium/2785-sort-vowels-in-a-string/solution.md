# 2785. Sort Vowels in a String

**Link:** https://leetcode.com/problems/sort-vowels-in-a-string/submissions/1767074133/

Given a 0-indexed string s, permute s to get a new string t such that: All consonants remain in their original places. More formally, if there is an index i with 0 <= i < s.length such that s[i] is a consonant, then t[i] = s[i]. The vowels must be sorted in the nondecreasing order of their ASCII values. More formally, for pairs of indices i, j with 0 <= i < j < s.length such that s[i] and s[j] are vowels, then t[i] must not have a higher ASCII value than t[j]. Return the resulting string. The vowels are 'a', 'e', 'i', 'o', and 'u', and they can appear in lowercase or uppercase. Consonants comprise all letters that are not vowels.

```java
        int j = 0;
        for (int i = 0; i < s.length(); i++) {
            if (isVowel(s.charAt(i))) {
                ans.append(temp.get(j));
                j++;
            } else {
                ans.append(s.charAt(i));
            }
        }
        
        return ans.toString();
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Data Structure

1. **Key Issues**: Attempt 1 lacks vowel sorting.  `temp` (presumably a sorted vowel list) isn't initialized or populated. The code only iterates through the input string, placing vowels from `temp` without ordering them.

2. **Evolution**: No subsequent attempts were provided to analyze improvement.  A correct solution would require sorting vowels before the iteration.

