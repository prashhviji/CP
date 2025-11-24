# 1018. Binary Prefix Divisible By 5

**Link:** https://leetcode.com/problems/binary-prefix-divisible-by-5/submissions/1838651616/

You are given a binary array nums (0-indexed). We define xi as the number whose binary representation is the subarray nums[0..i] (from most-significant-bit to least-significant-bit).

```java
class Solution {

    public List<Boolean> prefixesDivBy5(int[] nums) {
        List<Boolean> answer = new ArrayList<Boolean>();
        int prefix = 0;
        int length = nums.length;
        for (int i = 0; i < length; i++) {
            prefix = ((prefix << 1) + nums[i]) % 5;
            answer.add(prefix == 0);
        }
        return answer;
    }
}
```
