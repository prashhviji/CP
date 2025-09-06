# 3495. Minimum Operations to Make Array Elements Zero

**Link:** https://leetcode.com/problems/minimum-operations-to-make-array-elements-zero/

You are given a 2D array queries, where queries[i] is of the form [l, r]. Each queries[i] defines an array of integers nums consisting of elements ranging from l to r, both inclusive. In one operation, you can: Select two integers a and b from the array. Replace them with floor(a / 4) and floor(b / 4). Your task is to determine the minimum number of operations required to reduce all elements of the array to zero for each query. Return the sum of the results for all queries.

```java
            i++;
            base *= 2;
        }
        return cnt;
    }

    public long minOperations(int[][] queries) {
        long res = 0;
            int end = Math.min(base * 2 - 1, num);
            cnt += (long) ((i + 1) / 2) * (end - base + 1);
        long cnt = 0;
        int i = 1;
        int base = 1;
        while (base <= num) {
class Solution {

    private long get(int num) {
```
