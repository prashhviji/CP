# 3623. Count Number of Trapezoids I

**Link:** https://leetcode.com/problems/count-number-of-trapezoids-i/submissions/1844717000/

You are given a 2D integer array points, where points[i] = [xi, yi] represents the coordinates of the ith point on the Cartesian plane. A horizontal trapezoid is a convex quadrilateral with at least one pair of horizontal sides (i.e. parallel to the x-axis). Two lines are parallel if and only if they have the same slope. Return the  number of unique horizontal trapezoids that can be formed by choosing any four distinct points from points. Since the answer may be very large, return it modulo 109 + 7.

```java
        int MOD = 1000000007;
        Map<Integer, Long> map = new HashMap<>();
        for (int[] point : points){
            map.put(point[1], map.getOrDefault(point[1], 0L)+1);
        }
        long prev = 0;
        long curr = 0;
        long res = 0;
        for (long val : map.values()){
            curr = (val * (val - 1) / 2) % MOD;
            res = (res + prev * curr) % MOD;
            prev = (prev + curr) % MOD;
        }
        return (int)res;
    }
}
```
