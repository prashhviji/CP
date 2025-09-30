# 3027. Find the Number of Ways to Place People II

**Link:** https://leetcode.com/problems/find-the-number-of-ways-to-place-people-ii/submissions/1787425447/

You are given a 2D array points of size n x 2 representing integer coordinates of some points on a 2D-plane, where points[i] = [xi, yi]. We define the right direction as positive x-axis (increasing x-coordinate) and the left direction as negative x-axis (decreasing x-coordinate). Similarly, we define the up direction as positive y-axis (increasing y-coordinate) and the down direction as negative y-axis (decreasing y-coordinate) You have to place n people, including Alice and Bob, at these points such that there is exactly one person at every point. Alice wants to be alone with Bob, so Alice will build a rectangular fence with Alice's position as the upper left corner and Bob's position as the lower right corner of the fence (Note that the fence might not enclose any area, i.e. it can be a line). If any person other than Alice and Bob is either inside the fence or on the fence, Alice will be sad. Return the number of pairs of points where you can place Alice and Bob, such that Alice does not become sad on building the fence.

```java
                    pointB[0] < xMax &&
                    pointB[1] > yMin &&
                    pointB[1] < yMax
                ) {
                    ans++;
                    xMin = pointB[0];
                    yMin = pointB[1];
                }
            }
        }
        return ans;
    }
                if (
                    pointB[0] > xMin &&
            for (int j = i + 1; j < points.length; j++) {
                int[] pointB = points[j];

```
