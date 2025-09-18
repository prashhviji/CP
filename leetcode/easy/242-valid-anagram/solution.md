# 242. Valid Anagram

**Link:** https://leetcode.com/problems/valid-anagram/submissions/1774752675/

Given two strings s and t, return true if t is an anagram of s, and false otherwise.

```java
            return false;
        }

        char[] sArray = s.toCharArray();
        char[] tArray = t.toCharArray();

        Arrays.sort(sArray);
        Arrays.sort(tArray);

        return Arrays.equals(sArray, tArray);
    }
}

```

## Mistake Analysis

TAGS: Syntax Error, Logic Error

1. **Key Issues**: Attempt 1 has syntax errors; the code is not correctly formatted and is missing closing curly braces. The `if` statement checking string lengths is misplaced.  The core logic is correct, but the syntax prevents compilation.


2. **Evolution**: No evolution is shown as only one incomplete attempt is provided.  The corrected code would be syntactically sound and place the length check before sorting.

