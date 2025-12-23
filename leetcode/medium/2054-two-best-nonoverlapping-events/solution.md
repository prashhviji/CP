# 2054. Two Best Non-Overlapping Events

**Link:** https://leetcode.com/problems/two-best-non-overlapping-events/submissions/1863381826/

You are given a 0-indexed 2D integer array of events where events[i] = [startTimei, endTimei, valuei]. The ith event starts at startTimei and ends at endTimei, and if you attend this event, you will receive a value of valuei. You can choose at most two non-overlapping events to attend such that the sum of their values is maximized. Return this maximum sum. Note that the start time and end time is inclusive: that is, you cannot attend two events where one of them starts and the other ends at the same time. More specifically, if you attend an event with end time t, the next event must start at or after t + 1.

```java
        while (left < right) {
            int mid = left + (right - left) / 2;
            if (ends[mid] < target) {
                res = mid;
                left = mid + 1;
            } else {
                right = mid;
            }
        }

        return res;

    public int binary_search(int[] ends, int target, int right) {
        int left = 0;
        int res = -1;

    }
```
