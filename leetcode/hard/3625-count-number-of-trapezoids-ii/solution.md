# 3625. Count Number of Trapezoids II

**Link:** https://leetcode.com/problems/count-number-of-trapezoids-ii/submissions/1845917023/

You are given a 2D integer array points where points[i] = [xi, yi] represents the coordinates of the ith point on the Cartesian plane. Return the number of unique trapezoids that can be formed by choosing any four distinct points from points. A trapezoid is a convex quadrilateral with at least one pair of parallel sides. Two lines are parallel if and only if they have the same slope.

```java
                ans += (long) val * sum;
            }
        }

        return (int) ans;
    }

    private int gcd(int a, int b) {
        while (b != 0) {
            int t = a % b;
            a = b;
            b = t;
        }
        return Math.abs(a);
    }
}
```
