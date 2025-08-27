# 8. String to Integer (atoi)

**Link:** https://leetcode.com/problems/string-to-integer-atoi/description/

Implement the myAtoi(string s) function, which converts a string to a 32-bit signed integer. The algorithm for myAtoi(string s) is as follows: Whitespace: Ignore any leading whitespace (" "). Signedness: Determine the sign by checking if the next character is '-' or '+', assuming positivity if neither present. Conversion: Read the integer by skipping leading zeros until a non-digit character is encountered or the end of the string is reached. If no digits were read, then the result is 0. Rounding: If the integer is out of the 32-bit signed integer range [-231, 231 - 1], then round the integer to remain in the range. Specifically, integers less than -231 should be rounded to -231, and integers greater than 231 - 1 should be rounded to 231 - 1. Return the integer as the final result.

```java
        
        }
            i++;
        while (i < n && s.charAt(i) == ' ') {
        if (i == n) {
            return 0;
        }
        
        int sign = 1;
        if (s.charAt(i) == '+') {
            i++;
        } else if (s.charAt(i) == '-') {
            sign = -1;
            i++;
        }
        
        long res = 0;
        while (i < n && Character.isDigit(s.charAt(i))) {
```

## Mistake Analysis

TAGS: Syntax Error, Logic Error, Input Handling

1. **Key Issues**: Attempt 1 is incomplete and syntactically incorrect.  It lacks a complete conversion logic, sign handling, overflow check, and proper whitespace handling.  Several semicolons are missing, and variables are used before declaration.

2. **Evolution**: No further attempts provided, so no evolution can be assessed.  The incomplete code demonstrates a lack of understanding of fundamental string manipulation and integer conversion.

