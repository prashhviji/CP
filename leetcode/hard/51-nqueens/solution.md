# 51. N-Queens

**Link:** https://leetcode.com/problems/n-queens/submissions/1766364990/

The n-queens puzzle is the problem of placing n queens on an n x n chessboard such that no two queens attack each other. Given an integer n, return all distinct solutions to the n-queens puzzle. You may return the answer in any order. Each solution contains a distinct board configuration of the n-queens' placement, where 'Q' and '.' both indicate a queen and an empty space, respectively.

```java
                           boolean[] diag1,
                           boolean[] columns,
    private void backtrack(int row, int n, int[] board,

        return result;
    }
        
        backtrack(0, n, board, columns, diag1, diag2, result);
        boolean[] diag2 = new boolean [2* n-1];
        boolean[] columns = new boolean[n];
        boolean[] diag1 = new boolean[ 2* n-1];
        int[] board = new int[n];
        List<List<String>> result = new ArrayList<>();
    public List<List<String>> solveNQueens(int n) {
class Solution {

import java.util.*;
```
