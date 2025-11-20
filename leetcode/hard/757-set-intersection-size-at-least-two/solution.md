# 757. Set Intersection Size At Least Two

**Link:** https://leetcode.com/problems/set-intersection-size-at-least-two/submissions/1834869376/

You are given a 2D integer array intervals where intervals[i] = [starti, endi] represents all the integers from starti to endi inclusively. A containing set is an array nums where each interval from intervals has at least two integers in nums.

```java
            int s = intervals[t][0];
            int e = intervals[t][1];
            int m = todo[t];
            for (int p = s; p < s+m; ++p) {
                for (int i = 0; i <= t; ++i)
                    if (todo[i] > 0 && p <= intervals[i][1])
                        todo[i]--;
                ans++;
            }
        while (--t >= 0) {
        int[] todo = new int[intervals.length];
        Arrays.fill(todo, 2);
        int ans = 0, t = intervals.length;
                    a[0] != b[0] ? a[0]-b[0] : b[1]-a[1]);
    public int intersectionSizeTwo(int[][] intervals) {
        Arrays.sort(intervals, (a, b) ->
class Solution {
```
