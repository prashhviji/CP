# 1838. Frequency of the Most Frequent Element

**Link:** https://leetcode.com/problems/frequency-of-the-most-frequent-element/submissions/1807203883/

The frequency of an element is the number of times it occurs in an array. You are given an integer array nums and an integer k. In one operation, you can choose an index of nums and increment the element at that index by 1. Return the maximum possible frequency of an element after performing at most k operations.

```java
        
        for (int right = 0; right < nums.length; right++) {
            long target = nums[right];
            curr += target;
            
            while ((right - left + 1) * target - curr > k) {
                curr -= nums[left];
                left++;
            }
            
            ans = Math.max(ans, right - left + 1);
        int ans = 0;
        long curr = 0;
        Arrays.sort(nums);
        int left = 0;
class Solution {
    public int maxFrequency(int[] nums, int k) {
```
