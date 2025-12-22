# 960. Delete Columns to Make Sorted III

**Link:** https://leetcode.com/problems/delete-columns-to-make-sorted-iii/submissions/1862455386/

You are given an array of n strings strs, all of the same length. We may choose any deletion indices, and we delete all the characters in those indices for each string.

```java
                for (String row: A)
                    if (row.charAt(i) > row.charAt(j))
                        continue search;

                dp[i] = Math.max(dp[i], 1 + dp[j]);
            }

        int kept = 0;
        for (int x: dp)
            kept = Math.max(kept, x);
        return W - kept;
    }
}
```
