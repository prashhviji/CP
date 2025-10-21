# 3346. Maximum Frequency of an Element After Performing Operations I

**Link:** https://leetcode.com/problems/maximum-frequency-of-an-element-after-performing-operations-i/description/

You are given an integer array nums and two integers k and numOperations. You must perform an operation numOperations times on nums, where in each operation you: Select an index i that was not selected in any previous operations. Add an integer in the range [-k, k] to nums[i]. Return the maximum possible frequency of any element in nums after performing the operations.

```java

        for (int i = 1; i < maxVal; i++)
            count[i] += count[i - 1];

        int res = 0;
        for (int i = 0; i < maxVal; i++) {
            int left = Math.max(0, i - k);
            int right = Math.min(maxVal - 1, i + k);
            int total = count[right] - (left > 0 ? count[left - 1] : 0);
            int freq = count[i] - (i > 0 ? count[i - 1] : 0);
            res = Math.max(res, freq + Math.min(numOps, total - freq));
        }

        return res;
    }
}
```
