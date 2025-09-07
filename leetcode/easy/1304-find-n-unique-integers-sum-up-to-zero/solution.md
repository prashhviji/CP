# 1304. Find N Unique Integers Sum up to Zero

**Link:** https://leetcode.com/problems/find-n-unique-integers-sum-up-to-zero/submissions/1762240587/

Given an integer n, return any array containing n unique integers such that they add up to 0.

```java
        for(int i =1 ; i <= n/2; i++  ) {
            arr[index] = i;
        }
            index++;

            arr[index] = -i;
            index++;
        if(n%2 != 0){
            arr[index] =0;
        }
    }
        return arr;
}
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempt 1 has an incomplete loop and incorrect array manipulation.  The loop only iterates to `n/2`, and array indices are not correctly managed, leading to out-of-bounds and logic errors. The `index` variable isn't incremented consistently within the loop.

2. **Evolution**: No further attempts were provided to analyze improvement.

