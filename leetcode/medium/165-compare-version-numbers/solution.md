# 165. Compare Version Numbers

**Link:** https://leetcode.com/problems/compare-version-numbers/submissions/1775687538/

Given two version strings, version1 and version2, compare them. A version string consists of revisions separated by dots '.'. The value of the revision is its integer conversion ignoring leading zeros. To compare version strings, compare their revision values in left-to-right order. If one of the version strings has fewer revisions, treat the missing revision values as 0. Return the following: If version1 < version2, return -1. If version1 > version2, return 1. Otherwise, return 0.

```java
            int num2 = (i < v2.length)? Integer.parseInt(v2[i]) : 0;

            if(num1 < num2){
                return -1;
            }else if(num1 > num2){
                return 1;
            }
        }
            int num1 = (i < v1.length)? Integer.parseInt(v1[i]) : 0;

        for(int i =0; i<n; i++){
        int n = Math.max(v1.length, v2.length);

        return 0;
        
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Input Handling, Conditional Logic

1. **Key Issues**: Attempts 1-3 had syntax errors (missing semicolons, `num1` vs `num 1`). Attempt 1 incorrectly initialized `v1` and `v2` within the function and didn't iterate through all the numbers to compare.  The logic compared only one pair of numbers instead of iterating through all revisions.

2. **Evolution**: Attempts progressively corrected syntax errors. Attempt 4 finally fixed the logical error of only comparing one revision pair by introducing a loop iterating through all revisions.  Input handling of splitting version strings was improved across attempts.

