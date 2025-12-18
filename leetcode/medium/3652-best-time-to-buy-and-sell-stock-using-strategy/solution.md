# 3652. Best Time to Buy and Sell Stock using Strategy

**Link:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock-using-strategy/submissions/1859157566/

You are given two integer arrays prices and strategy, where: prices[i] is the price of a given stock on the ith day. strategy[i] represents a trading action on the ith day, where: -1 indicates buying one unit of the stock. 0 indicates holding the stock. 1 indicates selling one unit of the stock. You are also given an even integer k, and may perform at most one modification to strategy. A modification consists of: Selecting exactly k consecutive elements in strategy. Set the first k / 2 elements to 0 (hold). Set the last k / 2 elements to 1 (sell). The profit is defined as the sum of strategy[i] * prices[i] across all days. Return the maximum possible profit you can achieve.

```java
        long[] profitSum = new long[n + 1];
        long[] priceSum = new long[n + 1];
        for (int i = 0; i < n; i++) {
            profitSum[i + 1] = profitSum[i] + (long) prices[i] * strategy[i];
            priceSum[i + 1] = priceSum[i] + prices[i];
        }
        long res = profitSum[n];
        for (int i = k - 1; i < n; i++) {
            long leftProfit = profitSum[i - k + 1];
            long rightProfit = profitSum[n] - profitSum[i + 1];
            long changeProfit = priceSum[i + 1] - priceSum[i - k / 2 + 1];
            res = Math.max(res, leftProfit + changeProfit + rightProfit);
        }
        return res;
    }
}
```
