# 424. Longest Repeating Character Replacement

**Link:** https://leetcode.com/problems/longest-repeating-character-replacement/submissions/1865279824/

You are given a string s and an integer k. You can choose any character of the string and change it to any other uppercase English character. You can perform this operation at most k times. Return the length of the longest substring containing the same letter you can get after performing the above operations.

```java
        for(int right =0; right < s.length(); right ++){
        int result = 0;

        int[] freq = new int[26];
        int left = 0;
        int maxFreq = 0;
            int index = s.charAt(right) - 'A';
        }
            freq[index]++;
            maxFreq = Math.max(maxFreq, freq[index]);

            while((right - left +1) - maxFreq > k){
            result = Math.max(result, right - left +1);
            }
                freq[s.charAt(left) - 'A']--;
                left++;
    }
        return result;
    public int characterReplacement(String s, int k) {
}
class Solution {
```
