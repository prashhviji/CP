# 3494. Find the Minimum Amount of Time to Brew Potions

**Link:** https://leetcode.com/problems/find-the-minimum-amount-of-time-to-brew-potions/submissions/1796416639/

You are given two integer arrays, skill and mana, of length n and m, respectively. In a laboratory, n wizards must brew m potions in order. Each potion has a mana capacity mana[j] and must pass through all the wizards sequentially to be brewed properly. The time taken by the ith wizard on the jth potion is timeij = skill[i] * mana[j]. Since the brewing process is delicate, a potion must be passed to the next wizard immediately after the current wizard completes their work. This means the timing must be synchronized so that each wizard begins working on a potion exactly when it arrives. ​ Return the minimum amount of time required for the potions to be brewed properly.

```java
        int n = skill.length, m = mana.length;
        long[] done = new long[n + 1];
        
        for (int j = 0; j < m; ++j) {
            for (int i = 0; i < n; ++i) {
                done[i + 1] = Math.max(done[i + 1], done[i]) + (long) mana[j] * skill[i];
            }
            for (int i = n - 1; i > 0; --i) {
                done[i] = done[i + 1] - (long) mana[j] * skill[i];
            }
        }
        
        return done[n];
    }
}
```
