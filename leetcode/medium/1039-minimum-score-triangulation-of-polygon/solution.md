# 1039. Minimum Score Triangulation of Polygon

**Link:** https://leetcode.com/problems/minimum-score-triangulation-of-polygon/submissions/1785889377/

You have a convex n-sided polygon where each vertex has an integer value. You are given an integer array values where values[i] is the value of the ith vertex in clockwise order. Polygon triangulation is a process where you divide a polygon into a set of triangles and the vertices of each triangle must also be vertices of the original polygon. Note that no other shapes other than triangles are allowed in the division. This process will result in n - 2 triangles. You will triangulate the polygon. For each triangle, the weight of that triangle is the product of the values at its vertices. The total score of the triangulation is the sum of these weights over all n - 2 triangles. Return the minimum possible score that you can achieve with some triangulation of the polygon.

```java
            for (int i = 0; i + len - 1 < n; i++) {
                int j = i + len - 1;
                int best = Integer.MAX_VALUE;
                for (int k = i + 1; k < j; k++) {
                    int cost = dp[i][k] + dp[k][j] + values[i] * values[k] * values[j];
                    if(cost < best){
                dp[i][j] = best;
            }
                }
        for (int len = 3; len <= n; len++) {
        
                        best·‌=·‌cost;
                    }
        int[][] dp = new int[n][n];
        }
        return n == 0 ? 0 : dp[0][n-1];
    }
}
```
