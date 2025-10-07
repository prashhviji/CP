# 739. Daily Temperatures

**Link:** https://leetcode.com/problems/daily-temperatures/submissions/1793840354/

Given an array of integers temperatures represents the daily temperatures, return an array answer such that answer[i] is the number of days you have to wait after the ith day to get a warmer temperature. If there is no future day for which this is possible, keep answer[i] == 0 instead.

```java
        int[] answer = new int[n];
        Stack<Integer> stack = new Stack<>();  

        for(int i=0 ; i<n; i++){
    }
            while(!stack.isEmpty() && temperatures[i] > temperatures[stack.peek()]){
        }
                int idx = stack.pop();
            }
}
                answer[idx] = i-idx;
            stack.push(i);
        return answer; 

        int n = temperatures.length;
    public int[] dailyTemperatures(int[] temperatures) {
class Solution {
```
