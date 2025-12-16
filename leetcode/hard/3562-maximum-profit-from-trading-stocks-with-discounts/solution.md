# 3562. Maximum Profit from Trading Stocks with Discounts

**Link:** https://leetcode.com/problems/maximum-profit-from-trading-stocks-with-discounts/submissions/1857228172/

You are given an integer n, representing the number of employees in a company. Each employee is assigned a unique ID from 1 to n, and employee 1 is the CEO. You are given two 1-based integer arrays, present and future, each of length n, where: present[i] represents the current price at which the ith employee can buy a stock today. future[i] represents the expected price at which the ith employee can sell the stock tomorrow. The company's hierarchy is represented by a 2D integer array hierarchy, where hierarchy[i] = [ui, vi] means that employee ui is the direct boss of employee vi. Additionally, you have an integer budget representing the total funds available for investment. However, the company has a discount policy: if an employee's direct boss purchases their own stock, then the employee can buy their stock at half the original price (floor(present[v] / 2)). Return the maximum profit that can be achieved without exceeding the given budget.

```java
                dp1[i] = Math.max(
                    subProfit0[i],
                    subProfit1[i - dCost] + future[u] - dCost
                );
            }
            if (i >= cost) {
                dp0[i] = Math.max(
                    subProfit0[i],
                    subProfit1[i - cost] + future[u] - cost
                );
            }
        }

        return new Result(dp0, dp1, uSize);
    }
}
```
