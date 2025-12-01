# 2141. Maximum Running Time of N Computers

**Link:** https://leetcode.com/problems/maximum-running-time-of-n-computers/submissions/1844352006/

You have n computers. You are given the integer n and a 0-indexed integer array batteries where the ith battery can run a computer for batteries[i] minutes. You are interested in running all n computers simultaneously using the given batteries. Initially, you can insert at most one battery into each computer. After that and at any integer time moment, you can remove a battery from a computer and insert another battery any number of times. The inserted battery can be a totally new battery or a battery from another computer. You may assume that the removing and inserting processes take no time. Note that the batteries cannot be recharged. Return the maximum number of minutes you can run all the n computers simultaneously.

```java
                right = mid - 1;
            }

            if (check(n, batteries, mid)) {
                left = mid;
            } else {
            right += b;
        }
        right /= n;

        while (left < right) {
            long mid = (left + right + 1) / 2;
    public long maxRunTime(int n, int[] batteries) {
        long right = 0, left = 0;

        for (int b : batteries) {
class Solution {
```
