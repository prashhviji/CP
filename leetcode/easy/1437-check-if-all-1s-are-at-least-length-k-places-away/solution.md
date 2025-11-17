# 1437. Check If All 1's Are at Least Length K Places Away

**Link:** https://leetcode.com/problems/check-if-all-1s-are-at-least-length-k-places-away/submissions/1832453174/

Given an binary array nums and an integer k, return true if all 1's are at least k places away from each other, otherwise return false.

```java
class Solution {
    public boolean kLengthApart(int[] nums, int k) {
        int lastOccured = -1;
        for (int i = 0; i < nums.length; i++) {
            if (nums[i] == 1) {
                if (lastOccured != -1) {
                    int gap = i - lastOccured - 1;
                    if (gap < k) return false;
                }
                lastOccured = i;
            }
        }
        return true;
    }
}
```
