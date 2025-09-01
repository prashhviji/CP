# 1792. Maximum Average Pass Ratio

**Link:** https://leetcode.com/problems/maximum-average-pass-ratio/submissions/1755909010/

There is a school that has classes of students and each class will be having a final exam. You are given a 2D integer array classes, where classes[i] = [passi, totali]. You know beforehand that in the ith class, there are totali total students, but only passi number of students will pass the exam. You are also given an integer extraStudents. There are another extraStudents brilliant students that are guaranteed to pass the exam of any class they are assigned to. You want to assign each of the extraStudents students to a class in a way that maximizes the average pass ratio across all the classes. The pass ratio of a class is equal to the number of students of the class that will pass the exam divided by the total number of students of the class. The average pass ratio is the sum of pass ratios of all the classes divided by the number of the classes. Return the maximum possible average pass ratio after assigning the extraStudents students. Answers within 10-5 of the actual answer will be accepted.

```java
            double diff = findDiff(pass, total);
            int total = (int)arr[2] + 1;
            int pass = (int)arr[1] + 1;
        while(extraStudents>0){
            double arr[] = pq.poll();
        
        }
            pq.offer(new double[]{diff, pass, total});
            double diff = findDiff(pass, total);
            int total = arr[1];
            int pass = arr[0];
        for(int arr[] : classes){
    public double maxAverageRatio(int[][] classes, int extraStudents) {
        PriorityQueue<double[]> pq = new PriorityQueue<>( (a,b) -> Double.compare(b[0],a[0])); 
        
class Solution {
            pq.offer(new double[]{diff, pass, total});
```

## Mistake Analysis

TAGS: Logic Error, Data Structure, Algorithm Choice

1. **Key Issues**: Attempt 1 lacks a priority queue to efficiently select classes.  Attempt 2 uses a priority queue but has incomplete/incorrect logic for updating and adding elements, resulting in incorrect calculations. Both lack proper handling of the `extraStudents` decrement and average ratio calculation.

2. **Evolution**: Attempt 2 improved by using a priority queue (better algorithm choice), but the implementation contained significant logic and data structure handling errors.  Neither attempt correctly implements the core algorithm.

