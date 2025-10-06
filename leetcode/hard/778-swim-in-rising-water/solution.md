# 778. Swim in Rising Water

**Link:** https://leetcode.com/problems/swim-in-rising-water/submissions/1793279615/

You are given an n x n integer matrix grid where each value grid[i][j] represents the elevation at that point (i, j). It starts raining, and water gradually rises over time. At time t, the water level is t, meaning any cell with elevation less than equal to t is submerged or reachable. You can swim from a square to another 4-directionally adjacent square if and only if the elevation of both squares individually are at most t. You can swim infinite distances in zero time. Of course, you must stay within the boundaries of the grid during your swim. Return the minimum time until you can reach the bottom right square (n - 1, n - 1) if you start at the top left square (0, 0).

```java
    }
        }
        return lo;
            else lo = mid + 1;
            if (possible(grid, mid, m, n, directions)) hi = mid;
            int mid = lo + (hi - lo) / 2;
        while (lo < hi) {
        
                hi = Math.max(hi, val);
            for (int val : row)
        for (int[] row : grid)
        int lo = grid[0][0], hi = 0;
        
        int[][] directions = {{0,1}, {1,0}, {0,-1}, {-1,0}};
        int m = grid.length, n = grid[0].length;
    public int swimInWater(int[][] grid) {
class Solution {
```
