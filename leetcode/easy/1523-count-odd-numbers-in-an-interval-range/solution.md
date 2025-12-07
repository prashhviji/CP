# 1523. Count Odd Numbers in an Interval Range

**Link:** https://leetcode.com/problems/count-odd-numbers-in-an-interval-range/submissions/1849106315/

Given two non-negative integers low and high. Return the count of odd numbers between low and high (inclusive).

```java
class Solution {
    public int countOdds(int low, int high) {
       int nums=high-low+1;
       if(low%2!=0 && high%2!=0) return nums/2 + 1;
       else return nums/2;
    }
}
```
