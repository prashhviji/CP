# 3003. Maximize the Number of Partitions After Operations

**Link:** https://leetcode.com/problems/maximize-the-number-of-partitions-after-operations/submissions/1804354223/

You are given a string s and an integer k. First, you are allowed to change at most one index in s to another lowercase English letter. After that, do the following partitioning operation until s is empty: Choose the longest prefix of s containing at most k distinct characters. Delete the prefix from s and increase the number of partitions by one. The remaining characters (if any) in s maintain their initial order. Return an integer denoting the maximum number of resulting partitions after the operations by optimally choosing at most one index to change.

```java

        int maxVal = 0;
        for (int i = 0; i < n; i++) {
            int seg = left[i][0] + right[i][0] + 2;
            int totMask = left[i][1] | right[i][1];
            int totCount = Integer.bitCount(totMask);
            if (left[i][2] == k && right[i][2] == k && totCount < 26) {
                seg++;
            } else if (Math.min(totCount + 1, 26) <= k) {
                seg--;
            }
            maxVal = Math.max(maxVal, seg);
        }
        return maxVal;
    }
}
```
