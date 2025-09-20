# 875. Koko Eating Bananas

**Link:** https://leetcode.com/problems/koko-eating-bananas/submissions/1776614366/

Koko loves to eat bananas. There are n piles of bananas, the ith pile has piles[i] bananas. The guards have gone and will come back in h hours. Koko can decide her bananas-per-hour eating speed of k. Each hour, she chooses some pile of bananas and eats k bananas from that pile. If the pile has less than k bananas, she eats all of them instead and will not eat any more bananas during this hour. Koko likes to eat slowly but still wants to finish eating all the bananas before the guards return. Return the minimum integer k such that she can eat all the bananas within h hours.

```java
            }
                low = mid + 1; 
        }

        return low;
    }

    private boolean canEatAll(int[] piles, int h, int k) {
        int hours = 0;
        for (int pile : piles) {
            // ceil(pile / k) = (pile + k - 1) / k
            hours += (pile + k - 1) / k;
            if (hours > h) return false; 
        }
        return hours <= h;
    }
}

```
