# 295. Find Median from Data Stream

**Link:** https://leetcode.com/problems/find-median-from-data-stream/submissions/1835080606/

The median is the middle value in an ordered integer list. If the size of the list is even, there is no middle value, and the median is the mean of the two middle values.

```java
        else
            return small.peek();
    }

    public void addNum(int num) {
        if (even) {
            large.offer(num);
    public double findMedian() {
        if (even)
            return (small.peek() + large.peek()) / 2.0;
    private boolean even = true;

            small.offer(large.poll());
        } else {
            small.offer(num);
            large.offer(small.poll());
        }
```
