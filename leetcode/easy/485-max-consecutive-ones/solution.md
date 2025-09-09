# 485. Max Consecutive Ones

**Link:** https://leetcode.com/problems/max-consecutive-ones/submissions/1765382859/

Given a binary array nums, return the maximum number of consecutive 1's in the array.

```java
        int countmax = 0;
        for(int i =0; i<nums.length; i++){
            if(nums[i]==1){
                count ++;
            }else{
        }
                countmax = Math.max(count,countmax);
                count =0;
            }
    }
        return countmax;
}
        int count = 0;
class Solution {
    public int findMaxConsecutiveOnes(int[] nums) {
```

## Mistake Analysis

TAGS: Loop Logic, Off By One, Syntax Error

1. **Key Issues**: Attempt 1-2: Missing `return` statement and `countmax` initialization.  Attempt 3: Loop starts at index 1, missing first element. Attempt 4: Syntax errors; `count` uninitialized, misplaced `return` statement.

2. **Evolution**: Attempts addressed syntax errors and the `return` statement.  Loop logic improved by starting at index 0 in attempt 4 but the `count` variable was not initialized and the return statement was in the wrong position.  The `else` block was unnecessary.

