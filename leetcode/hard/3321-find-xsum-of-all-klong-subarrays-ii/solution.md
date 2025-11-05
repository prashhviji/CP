# 3321. Find X-Sum of All K-Long Subarrays II

**Link:** https://leetcode.com/problems/find-x-sum-of-all-k-long-subarrays-ii/submissions/1821581109/

You are given an array nums of n integers and two integers k and x. The x-sum of an array is calculated by the following procedure: Count the occurrences of all elements in the array. Keep only the occurrences of the top x most frequent elements. If two elements have the same number of occurrences, the element with the bigger value is considered more frequent. Calculate the sum of the resulting array. Note that if an array has less than x distinct elements, its x-sum is the sum of the array. Return an integer array answer of length n - k + 1 where answer[i] is the x-sum of the subarray nums[i..i + k - 1].

```java
            small.add(p);
            }
        } else {
                small.add(toRemove);
                result -= (long) toRemove.first * toRemove.second;
                large.remove(toRemove);
                Pair toRemove = large.first();
            large.add(p);
            if (large.size() > x) {
            result += (long) p.first * p.second;
        if (large.size() < x || p.compareTo(large.first()) > 0) {
    private void internalInsert(Pair p) {

    }
        return result;
    public long get() {

    }
```
