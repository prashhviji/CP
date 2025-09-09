# 2327. Number of People Aware of a Secret

**Link:** https://leetcode.com/problems/number-of-people-aware-of-a-secret/submissions/1765164941/

On day 1, one person discovers a secret. You are given an integer delay, which means that each person will share the secret with a new person every day, starting from delay days after discovering the secret. You are also given an integer forget, which means that each person will forget the secret forget days after discovering it. A person cannot share the secret on the same day they forgot it, or on any day afterwards. Given an integer n, return the number of people who know the secret at the end of day n. Since the answer may be very large, return it modulo 109 + 7.

```java
                knowCnt = (knowCnt - first[1] + MOD) % MOD;
                shareCnt = (shareCnt + first[1]) % MOD;
                share.add(first);
        for (int i = 2; i <= n; i++) {
            if (!know.isEmpty() && know.peekFirst()[0] == i - delay) {
                int[] first = know.pollFirst();
        int shareCnt = 0;

        Deque<int[]> share = new LinkedList<>();
        know.add(new int[] { 1, 1 });
        int knowCnt = 1;
        Deque<int[]> know = new LinkedList<>();
    private static final int MOD = 1000000007;

    public int peopleAwareOfSecret(int n, int delay, int forget) {

class Solution {
```
