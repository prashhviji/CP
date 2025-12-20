# 944. Delete Columns to Make Sorted

**Link:** https://leetcode.com/problems/delete-columns-to-make-sorted/submissions/1860779137/

You are given an array of n strings strs, all of the same length. The strings can be arranged such that there is one on each line, making a grid.

```java
    public int minDeletionSize(String[] s) {
        int n = s.length, m = s[0].length();
        int count = 0;

        for (int row_concrete = 0; row_concrete < m; row_concrete++) {
            for (int row = 1; row < n; row++) {
                if (s[row].charAt(row_concrete) < s[row - 1].charAt(row_concrete)) {
                    count++;
                    break;
                }
            }
        }

        return count;
    }
}
```
