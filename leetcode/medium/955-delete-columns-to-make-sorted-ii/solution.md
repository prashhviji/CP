# 955. Delete Columns to Make Sorted II

**Link:** https://leetcode.com/problems/delete-columns-to-make-sorted-ii/submissions/1861679676/

You are given an array of n strings strs, all of the same length. We may choose any deletion indices, and we delete all the characters in those indices for each string.

```python
                if not sorted_pairs[i] and strs[i][col] > strs[i + 1][col]:
                    bad = True
                    break

            if bad:
                delCount += 1
                continue

            for i in range(n - 1):
                if not sorted_pairs[i] and strs[i][col] < strs[i + 1][col]:
                    sorted_pairs[i] = True

            if all(sorted_pairs):
                break

        return delCount
```
