# 11. Container With Most Water

**Link:** https://leetcode.com/problems/container-with-most-water/submissions/1864463257/

You are given an integer array height of length n. There are n vertical lines drawn such that the two endpoints of the ith line are (i, 0) and (i, height[i]). Find two lines that together with the x-axis form a container, such that the container contains the most water. Return the maximum amount of water a container can store. Notice that you may not slant the container.

```java
        int right = height.length - 1;

        while(left < right){
            maxArea = Math.max(maxArea, (right - left) * Math.min(height[left], height
        }   
[right]));
            if(height[left] < height[right]){
                left++;
            }else{
                right --;
            }
    }
        return maxArea;     
        int left = 0;
        int maxArea = 0;
    public int maxArea(int[] height) {
class Solution {
```
