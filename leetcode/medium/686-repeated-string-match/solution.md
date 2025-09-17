# 686. Repeated String Match

**Link:** https://leetcode.com/problems/repeated-string-match/submissions/1773405438/

Given two strings a and b, return the minimum number of times you should repeat string a so that string b is a substring of it. If it is impossible for b​​​​​​ to be a substring of a after repeating it, return -1. Notice: string "abc" repeated 0 times is "", repeated 1 time is "abc" and repeated 2 times is "abcabc".

```java
                }
                    count++;

                if(start >= A.length() && j< B.length()){
                    start %= A.length();
                j++;
                start++;

                while(j < B.length() && A.charAt(start) == B.charAt(j)){
                int j =0;
                int start = i;
                int count = 1;
            if(A.charAt(i)  == B.charAt(0)){
        for(int i =0; i<A.length(); i++){
        
    public int repeatedStringMatch(String A, String B) {
class Solution {
```

## Mistake Analysis

TAGS: Loop Logic, Conditional Logic, Logic Error

1. **Key Issues**: Attempt 1 and 2 have misplaced `count++`, incrementing even when not wrapping around `A`.  Attempt 3 has incorrect conditional logic and placement of loop initializer. None handle cases where `A` is shorter than `B`.

2. **Evolution**: Attempts show progress in correctly placing `count++` within the wrap-around conditional. However, fundamental logic flaws regarding string matching and handling edge cases persist.

