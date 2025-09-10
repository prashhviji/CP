# 46. Permutations

**Link:** https://leetcode.com/problems/permutations/submissions/1765649964/

Given an array nums of distinct integers, return all the possible permutations. You can return the answer in any order.

```java
        if(current.size() == nums.length){
            result.add(new ArrayList <> (current));
        }
            return;
        for(int i=0;i<nums.length; i++){
            if(!used[i]){
                used[i] = true;
    }
    private void backtrack(int[]nums, List<Integer> current, boolean[] used,
List<List<Integer>> result){
        return result;

        List<List<Integer>> result = new ArrayList<>();
        boolean used[] = new boolean[nums.length];
        backtrack(nums, new ArrayList<>(),used,result);
class Solution {
    public List<List<Integer>> permute(int[] nums) {
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Loop Logic

1. **Key Issues**: Attempt 1 and 2 have syntax errors (missing `}` and incomplete function definition). Attempt 3 fixes syntax but lacks backtracking: `used[i] = false;` and `current.remove(...)` are crucial for exploring all permutations but are only partially implemented.

2. **Evolution**: Attempts show progress in fixing syntax errors.  However, the core logic error of incomplete backtracking remained until Attempt 3, where it's partially addressed.

