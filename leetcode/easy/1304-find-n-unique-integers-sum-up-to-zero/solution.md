# 1304. Find N Unique Integers Sum up to Zero

**Link:** https://leetcode.com/problems/find-n-unique-integers-sum-up-to-zero/submissions/1762241231/

Given an integer n, return any array containing n unique integers such that they add up to 0.

```java
        for(int i =1 ; i <= n/2; i++  ) {
            arr[index] = i;
        }
            index++;

            arr[index] = -i;
            index++;
        
    }
        return arr;
        int index =0;

        int arr[] = new int[n];
}
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Array Bounds

1. **Key Issues**: Attempt 1 has syntax errors (missing closing brace for the `for` loop and function), and a logic error in its attempt to create pairs of positive and negative integers. It also doesn't handle odd `n` correctly and has an uninitialized `index` variable.  Array bounds are not explicitly checked, creating a potential risk for out-of-bounds access.

2. **Evolution**: No evolution is shown as only one incomplete attempt is provided.

