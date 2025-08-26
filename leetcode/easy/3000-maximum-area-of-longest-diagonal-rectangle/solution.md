# 3000. Maximum Area of Longest Diagonal Rectangle

**Link:** https://leetcode.com/problems/maximum-area-of-longest-diagonal-rectangle/submissions/1749321565/

You are given a 2D 0-indexed integer array dimensions. For all indices i, 0 <= i < dimensions.length, dimensions[i][0] represents the length and dimensions[i][1] represents the width of the rectangle i. Return the area of the rectangle having the longest diagonal. If there are multiple rectangles with the longest diagonal, return the area of the rectangle having the maximum area.

```java
            int area = len * wid;

            if (diag > max_diag) {
                max_diag = diag;
                max_area = area;
            } else if (diag == max_diag) {
                max_area = Math.max(max_area, area);
            }
            int wid = dimensions[i][1];   
            int diag = len * len + wid * wid;

        for (int i = 0; i < dimensions.length; i++) {
            int len = dimensions[i][0];   
        int max_area = 0;  
    public int areaOfMaxDiagonal(int[][] dimensions) {
        int max_diag = 0;   
class Solution {
```

## Mistake Analysis

TAGS: Syntax Error, Logic Error, Conditional Logic

1. **Key Issues**: Attempt 1 has syntax errors (variable declarations misplaced, code outside method).  The diagonal calculation is incorrect (`diag = len * len + wid * wid` should be `diag = Math.sqrt(len*len + wid*wid)`), and the conditional logic for updating `max_area` is inefficient and potentially incorrect.

2. **Evolution**: No evolution is shown as only a fragment of a single attempt is provided.  The code is incomplete and uncompilable.

