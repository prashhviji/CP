# 4. Median of Two Sorted Arrays

**Link:** https://leetcode.com/problems/median-of-two-sorted-arrays/submissions/1777724465/

Given two sorted arrays nums1 and nums2 of size m and n respectively, return the median of the two sorted arrays. The overall run time complexity should be O(log (m+n)).

```java
            } else {
            if (i < m && (j >= n || nums1[i] <= nums2[j])) {
                curr = nums1[i];
                i++;
            prev = curr;

        int i = 0, j = 0;    
        int prev = 0, curr = 0;

        for (int step = 0; step <= mid; step++) {

                curr = nums2[j];
                j++;
            }
        }

        if (total % 2 == 1) {
            return curr;
```

## Mistake Analysis

TAGS: Algorithm Choice, Logic Error, Conditional Logic

1. **Key Issues**: Attempt 1 is an incomplete implementation of a binary search approach to find the median.  The code lacks crucial logic for handling the cases where the partition points lead to correct median calculation, and the `IllegalArgumentException` is improperly placed.  Conditional logic for adjusting `high` and `low` is incomplete.

2. **Evolution**: No evolution is shown as only one incomplete attempt is provided.  The provided code snippet is missing essential parts of the algorithm, rendering any evolution analysis impossible.

