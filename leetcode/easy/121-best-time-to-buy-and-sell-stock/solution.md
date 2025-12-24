# 121. Best Time to Buy and Sell Stock

**Link:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock/submissions/1864483840/

You are given an array prices where prices[i] is the price of a given stock on the ith day. You want to maximize your profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock. Return the maximum profit you can achieve from this transaction. If you cannot achieve any profit, return 0.

```java
    public int maxProfit(int[] prices) {
        int buyprice = prices[0];
        int profit = 0;

        for(int i = 1; i <prices.length; i++){
            if(buyprice > prices[i]){
        }
        
                buyprice = prices[i]; 
            }else{
                profit = Math.max(profit , prices[i] - buyprice);
            }
    }
        return profit;
}
class Solution {
```
