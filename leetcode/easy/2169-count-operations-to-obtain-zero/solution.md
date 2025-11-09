# 2169. Count Operations to Obtain Zero

**Link:** https://leetcode.com/problems/count-operations-to-obtain-zero/submissions/1825236223/

You are given two non-negative integers num1 and num2. In one operation, if num1 >= num2, you must subtract num2 from num1, otherwise subtract num1 from num2.

```java
class Solution {

    public int countOperations(int num1, int num2) {
        int res = 0; 
        while (num1 != 0 && num2 != 0) {
            res += num1 / num2;
            num1 %= num2;
            int temp = num1;
            num1 = num2;
            num2 = temp;
        }
        return res;
    }
}
```
