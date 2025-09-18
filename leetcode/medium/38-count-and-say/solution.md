# 38. Count and Say

**Link:** https://leetcode.com/problems/count-and-say/description/

The count-and-say sequence is a sequence of digit strings defined by the recursive formula: countAndSay(1) = "1" countAndSay(n) is the run-length encoding of countAndSay(n - 1).

```java
        for (int i = 1; i < s.length(); i++) {
            if (s.charAt(i) == s.charAt(i - 1)) {
                count++;
            } else {
                sb.append(count).append(s.charAt(i - 1));
                count = 1;
            }
        }

        int count = 1;

        StringBuilder sb = new StringBuilder();
    private String describe(String s) {

    }
        return result;
        sb.append(count).append(s.charAt(s.length() - 1));
```
