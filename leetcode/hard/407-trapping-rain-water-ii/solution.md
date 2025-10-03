# 407. Trapping Rain Water II

**Link:** https://leetcode.com/problems/trapping-rain-water-ii/submissions/1790400454/

Given an m x n integer matrix heightMap representing the height of each unit cell in a 2D elevation map, return the volume of water it can trap after raining.

```java
        }
        for (int j = 0; j < n; j++) {
            visited[i][0] = visited[i][n - 1] = true;
            pq.offer(new int[] { heightMap[i][0], i, 0 });
            pq.offer(new int[] { heightMap[i][n - 1], i, n - 1 });
        for (int i = 0; i < m; i++) {

        boolean[][] visited = new boolean[m][n];
        PriorityQueue<int[]> pq = new PriorityQueue<>((a, b) -> a[0] - b[0]);

    public int trapRainWater(int[][] heightMap) {
        int m = heightMap.length, n = heightMap[0].length;
        if (m < 3 || n < 3)
            return 0;
import java.util.PriorityQueue;

class Solution {
```
