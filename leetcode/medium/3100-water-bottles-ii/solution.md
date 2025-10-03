# 3100. Water Bottles II

**Link:** https://leetcode.com/problems/water-bottles-ii/submissions/1789918214/

You are given two integers numBottles and numExchange. numBottles represents the number of full water bottles that you initially have. In one operation, you can perform one of the following operations: Drink any number of full water bottles turning them into empty bottles. Exchange numExchange empty bottles with one full water bottle. Then, increase numExchange by one.

```java
class Solution {
    public int maxBottlesDrunk(int numBottles, int x) {
        int ans = numBottles;
        while (numBottles >= x) {
            numBottles -= x - 1;
            x++;
            ans++;
        }
        return ans;
    }
}
```
