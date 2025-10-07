# 22. Generate Parentheses

**Link:** https://leetcode.com/problems/generate-parentheses/submissions/1793795313/

Given n pairs of parentheses, write a function to generate all combinations of well-formed parentheses.

```java
            current.append(')');
            current.deleteCharAt(current.length() - 1); // backtrack
        }

        if (close < open) {
            backtrack(n, open + 1, close, current, result);
            current.append('(');
        if (open < n) {

            backtrack(n, open, close + 1, current, result);
            current.deleteCharAt(current.length() - 1); // backtrack
        }
    }

    
}

```
