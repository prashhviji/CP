# 29. Divide Two Integers

**Link:** https://leetcode.com/problems/divide-two-integers/editorial/

Given two integers dividend and divisor, divide two integers without using multiplication, division, and mod operator.

```java
        while(n>=d)
        {
        int ans = 0;
        if(dividend>0 && divisor<0) sign = -1;
        if(dividend<0 && divisor>0) sign = -1;

        long n = Math.abs((long)dividend);
        long d = Math.abs((long)divisor);
        if(dividend == -1) return -dividend;
        int sign = 1;
        }
        if(divisor == 1) return dividend;
            return Integer.MAX_VALUE;
    public int divide(int dividend, int divisor) {
        if(dividend == divisor) return 1;
        if (dividend == Integer.MIN_VALUE && divisor == -1) {
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Loop Logic

1. **Key Issues**: Attempt 1 has numerous syntax errors (missing braces, misplaced code).  The `while` loop lacks a body and increment/decrement step. Conditional logic for sign handling is incomplete and improperly placed. The return statement `return Integer.MAX_VALUE` is outside the function and always executes.

2. **Evolution**: No evolution is shown as only an incomplete attempt is provided.  The code is not functional.

