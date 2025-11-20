# 215. Kth Largest Element in an Array

**Link:** https://leetcode.com/problems/kth-largest-element-in-an-array/submissions/1835096266/

Given an integer array nums and an integer k, return the kth largest element in the array. Note that it is the kth largest element in the sorted order, not the kth distinct element. Can you solve it without sorting?

```java
class Solution {
    public int findKthLargest(int[] nums, int k) {
        PriorityQueue<Integer> pq = new PriorityQueue<>();
        for(int i =0; i < k; i++){
            pq.offer(nums[i]);
        }
        for(int i =k; i < nums.length; i++){
            if(nums[i] > pq.peek()){
                pq.poll();
                pq.offer(nums[i]);
            }
        }
        return pq.peek();
    }
}
```
