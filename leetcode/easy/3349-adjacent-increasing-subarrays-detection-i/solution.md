# 3349. Adjacent Increasing Subarrays Detection I

**Link:** https://leetcode.com/problems/adjacent-increasing-subarrays-detection-i/submissions/1801682014/

Given an array nums of n integers and an integer k, determine whether there exist two adjacent subarrays of length k such that both subarrays are strictly increasing. Specifically, check if there are two subarrays starting at indices a and b (a < b), where: Both subarrays nums[a..a + k - 1] and nums[b..b + k - 1] are strictly increasing. The subarrays must be adjacent, meaning b = a + k. Return true if it is possible to find two such subarrays, and false otherwise.

```java
            streak[i] = count;
        }

        for (int i = k; i < n; i++) {
            if (streak[i] >= k && streak[i - k] >= k) {
                return true;
            }
        }

        return false;
    }
}

```
