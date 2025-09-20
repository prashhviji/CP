# 74. Search a 2D Matrix

**Link:** https://leetcode.com/problems/search-a-2d-matrix/submissions/1776595446/

You are given an m x n integer matrix matrix with the following two properties: Each row is sorted in non-decreasing order. The first integer of each row is greater than the last integer of the previous row. Given an integer target, return true if target is in matrix or false otherwise. You must write a solution in O(log(m * n)) time complexity.

```java
       
        for(int i = 0; i< n; i++){
            for(int j =0; j<m; j++){
        }
                if(matrix[i][j] == target){
            }
                    return true;
                
                }
    }
        return false;
        int m = matrix[0].length;
        int n = matrix.length;
    public boolean searchMatrix(int[][] matrix, int target) {
}
```

## Mistake Analysis

TAGS: Loop Logic, Conditional Logic, Algorithm Choice

1. **Key Issues**: All attempts use nested loops (O(m*n) time), failing the time complexity requirement.  Conditional logic within the loops is incomplete and incorrectly structured; it returns prematurely.  No binary search approach is attempted.

2. **Evolution**: Attempts show minor syntax improvements (removing unnecessary semicolons, fixing return type), but the core flawed algorithm remains unchanged.  The problem's logarithmic time complexity requirement is completely ignored.

