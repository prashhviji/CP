# 15. 3Sum

**Link:** https://leetcode.com/problems/3sum/submissions/1863403397/

Given an integer array nums, return all the triplets [nums[i], nums[j], nums[k]] such that i != j, i != k, and j != k, and nums[i] + nums[j] + nums[k] == 0. Notice that the solution set must not contain duplicate triplets.

```java
                long sum = (long)nums[i]+ nums[left] + nums[right];
                if(sum == target){
                result.add(Arrays.asList(nums[i] , nums[left] , nums[right]));

                while (left < right && nums[left] == nums[left+1]) left++;
                        while (left < right && nums[right] == nums[right-1]) right--;

            while(left < right){
            int right =nums.length -1;
        for(int i=0; i<nums.length-2; i++){
            if (i > 0 && nums[i] == nums[i-1]) continue;
            int left = i+1;
        List<List<Integer>> result = new ArrayList<>();
        int target =0;
        Arrays.sort(nums);
class Solution {
    public List<List<Integer>> threeSum(int[] nums) {
```
