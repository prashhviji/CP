# 3578. Count Partitions With Max-Min Difference at Most K

**Link:** https://leetcode.com/problems/count-partitions-with-max-min-difference-at-most-k/submissions/1848585894/

You are given an integer array nums and an integer k. Your task is to partition nums into one or more non-empty contiguous segments such that in each segment, the difference between its maximum and minimum elements is at most k. Return the total number of ways to partition nums under this condition. Since the answer may be too large, return it modulo 109 + 7.

```java

                j++;
            }

            long left = (j > 0 ? prefix[j - 1] : 0);
            dp[i + 1] = (prefix[i] - left + mod) % mod;

            prefix[i + 1] = (prefix[i] + dp[i + 1]) % mod;
        }

        return (int) dp[n];
    }
}
```
