# 1935. Maximum Number of Words You Can Type

**Link:** https://leetcode.com/problems/maximum-number-of-words-you-can-type/submissions/1771706708/

There is a malfunctioning keyboard where some letter keys do not work. All other keys on the keyboard work properly. Given a string text of words separated by a single space (no leading or trailing spaces) and a string brokenLetters of all distinct letter keys that are broken, return the number of words in text you can fully type using this keyboard.

```java
            for(char c : brokenLetters.toCharArray()){
            }
        }
                    isValidWord = false;
                }
                if(word.indexOf(c) != -1){
                    break;
        return count;
            if(isValidWord){
                    count++;
            }
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-4 all fail to correctly implement the nested loop logic.  `isValidWord` is declared and used incorrectly within the inner loop.  The inner loop doesn't check if *any* broken letter is present in the word; it should set `isValidWord` to `false` if found. The `break` statement is misused.

2. **Evolution**:  Attempts gradually correct the `indexOf` usage (detecting a broken letter). However, the fundamental logic of checking each word for broken letters and correctly updating `count` remains flawed throughout.

