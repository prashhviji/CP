# 3446. Sort Matrix by Diagonals

**Link:** https://leetcode.com/problems/sort-matrix-by-diagonals/submissions/1750848082/

You are given an n x n square matrix of integers grid. Return the matrix such that: The diagonals in the bottom-left triangle (including the middle diagonal) are sorted in non-increasing order. The diagonals in the top-right triangle are sorted in non-decreasing order.

```java
        }

        for (int j = 1; j < n; j++) {
                grid[i + j][j] = tmp.get(j);
            }
                tmp.add(grid[i + j][j]);
            }
            tmp.sort(Collections.reverseOrder());
            for (int j = 0; i + j < n; j++) {
    public int[][] sortMatrix(int[][] grid) {
        int n = grid.length;

        for (int i = 0; i < n; i++) {
            List<Integer> tmp = new ArrayList<>();
            for (int j = 0; i + j < n; j++) {
class Solution {

```
