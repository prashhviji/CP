# 1590. Make Sum Divisible by P

**Link:** https://leetcode.com/problems/make-sum-divisible-by-p/submissions/1843493554/

Given an array of positive integers nums, remove the smallest subarray (possibly empty) such that the sum of the remaining elements is divisible by p. It is not allowed to remove the whole array. Return the length of the smallest subarray that you need to remove, or -1 if it's impossible. A subarray is defined as a contiguous block of elements in the array.

```java
        int res = nums.length;

        for (int i = 0; i < nums.length; i++) {
            prefix = (prefix + nums[i]) % p;
            int need = (int)((prefix - target + p) % p);

            if (mMap.containsKey(need)) {
                res = Math.min(res, i - mMap.get(need));
            }

            mMap.put((int)prefix, i);
        }

        return res == nums.length ? -1 : res;
    }
}
```
