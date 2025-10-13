# 2273. Find Resultant Array After Removing Anagrams

**Link:** https://leetcode.com/problems/find-resultant-array-after-removing-anagrams/submissions/1800598143/

You are given a 0-indexed string array words, where words[i] consists of lowercase English letters. In one operation, select any index i such that 0 < i < words.length and words[i - 1] and words[i] are anagrams, and delete words[i] from words. Keep performing this operation as long as you can select an index that satisfies the conditions. Return words after performing all operations. It can be shown that selecting the indices for each operation in any arbitrary order will lead to the same result.

```java
            freq[ch - 'a']++;
        }
        for (char ch : word2.toCharArray()) {
            freq[ch - 'a']--;
        }
        for (int x : freq) {
            if (x != 0) {
                return false;
            }
        }
        return true;
    }
}
```
