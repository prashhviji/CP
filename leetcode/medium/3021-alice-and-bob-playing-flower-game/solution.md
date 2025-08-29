# 3021. Alice and Bob Playing Flower Game

**Link:** https://leetcode.com/problems/alice-and-bob-playing-flower-game/submissions/1752532290/

Alice and Bob are playing a turn-based game on a field, with two lanes of flowers between them. There are x flowers in the first lane between Alice and Bob, and y flowers in the second lane between them. The game proceeds as follows: Alice takes the first turn. In each turn, a player must choose either one of the lane and pick one flower from that side. At the end of the turn, if there are no flowers left at all, the current player captures their opponent and wins the game. Given two integers, n and m, the task is to compute the number of possible pairs (x, y) that satisfy the conditions: Alice must win the game according to the described rules. The number of flowers x in the first lane must be in the range [1,n]. The number of flowers y in the second lane must be in the range [1,m]. Return the number of possible pairs (x, y) that satisfy the conditions mentioned in the statement.

```java
class Solution {

    public long flowerGame(int n, int m) {
        return ((long) m * n) / 2;
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice

1. **Key Issues**: Attempt 1 incorrectly assumes a simple division will determine the winner. It ignores the turn-based nature and the strategic choices involved in picking flowers from either lane.  The formula doesn't account for who wins based on the last flower.

2. **Evolution**: No subsequent attempts provided, preventing analysis of improvement.  A correct solution would require a recursive or iterative approach modeling the game's turns.

