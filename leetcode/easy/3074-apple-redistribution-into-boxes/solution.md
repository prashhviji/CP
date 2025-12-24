# 3074. Apple Redistribution into Boxes

**Link:** https://leetcode.com/problems/apple-redistribution-into-boxes/submissions/1864322141/

You are given an array apple of size n and an array capacity of size m. There are n packs where the ith pack contains apple[i] apples. There are m boxes as well, and the ith box has a capacity of capacity[i] apples. Return the minimum number of boxes you need to select to redistribute these n packs of apples into boxes. Note that, apples from the same pack can be distributed into different boxes.

```java
        Integer[] capArray = new Integer[capacity.length];
        for (int i = 0; i < capacity.length; i++) {
            capArray[i] = capacity[i];
        }

        Arrays.sort(capArray, Collections.reverseOrder());

        int need = 0;
        while (sum > 0) {
            sum -= capArray[need];
            need += 1;
        }

        return need;
    }
}
```
