# 2300. Successful Pairs of Spells and Potions

**Link:** https://leetcode.com/problems/successful-pairs-of-spells-and-potions/submissions/1795420817/

You are given two positive integer arrays spells and potions, of length n and m respectively, where spells[i] represents the strength of the ith spell and potions[j] represents the strength of the jth potion. You are also given an integer success. A spell and potion pair is considered successful if the product of their strengths is at least success. Return an integer array pairs of length n where pairs[i] is the number of potions that will form a successful pair with the ith spell.

```java
            while (left <= right) {
                int mid = (left + right) / 2;
                if (sp * potions[mid] >= success) {
                    index = mid;
                    right = mid - 1;
                } else {
                    left = mid + 1;
                }
            }
            
            ans[i] = (index == -1) ? 0 : (m - index);
        }
        
        return ans;
    }
}
```
