# 14. Longest Common Prefix

**Link:** https://leetcode.com/problems/longest-common-prefix/submissions/1773175365/

Write a function to find the longest common prefix string amongst an array of strings. If there is no common prefix, return an empty string "".

```java
        for(int i =0; i< first.length(); i++){
            char c = first.charAt(i);
        }

        String first = strs[0];

            for(int j = 0; j< strs.length; j++){
                if(i >= strs[j].length() || strs[j].charAt(i) != c){
                    return first.substring(0,i);
                }
            }
        
        }
            return "";
        if(strs == null || strs.length == 0){
        return first;
    }
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-5 had logic errors in their inner loop.  The `if` condition prematurely returned a substring instead of checking all strings. `i` was not updated correctly to reflect the common prefix length. Attempt 6 had a variable declaration order issue.

2. **Evolution**: Attempts incrementally improved by correctly identifying the `charAt` method and fixing the comparison condition in the inner loop (`i >= strs[j].length()`).  However, the fundamental logic error in the return statement persisted until attempt 6.  Even then, the code is still incomplete and will fail on edge cases.

