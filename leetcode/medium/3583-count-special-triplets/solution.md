# 3583. Count Special Triplets

**Link:** https://leetcode.com/problems/count-special-triplets/submissions/1851248223/

You are given an integer array nums. A special triplet is defined as a triplet of indices (i, j, k) such that: 0 <= i < j < k < n, where n = nums.length nums[i] == nums[j] * 2 nums[k] == nums[j] * 2 Return the total number of special triplets in the array. Since the answer may be large, return it modulo 109 + 7.

```java
        for (int v : nums) {
            int target = v * 2;
            int lCnt = numPartialCnt.getOrDefault(target, 0);
            numPartialCnt.put(v, numPartialCnt.getOrDefault(v, 0) + 1);
            int rCnt =
                numCnt.getOrDefault(target, 0) -
                numPartialCnt.getOrDefault(target, 0);
            ans = (ans + (long) lCnt * rCnt) % MOD;
        }

        return (int) ans;
    }
}
```
