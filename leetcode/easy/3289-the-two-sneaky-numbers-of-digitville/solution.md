# 3289. The Two Sneaky Numbers of Digitville

**Link:** https://leetcode.com/problems/the-two-sneaky-numbers-of-digitville/submissions/1816461464/

In the town of Digitville, there was a list of numbers called nums containing integers from 0 to n - 1. Each number was supposed to appear exactly once in the list, however, two mischievous numbers sneaked in an additional time, making the list longer than usual. As the town detective, your task is to find these two sneaky numbers. Return an array of size two containing the two numbers (in any order), so peace can return to Digitville.

```java

    public int[] getSneakyNumbers(int[] nums) {
        List<Integer> res = new ArrayList<>();
        Map<Integer, Integer> count = new HashMap<>();
        for (int x : nums) {
            int c = count.getOrDefault(x, 0) + 1;
            count.put(x, c);
            if (c == 2) {
                res.add(x);
            }
        }
        return res.stream().mapToInt(Integer::intValue).toArray();
    }
}
class Solution {
```
