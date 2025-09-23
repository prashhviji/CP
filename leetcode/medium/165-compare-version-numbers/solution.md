# 165. Compare Version Numbers

**Link:** https://leetcode.com/problems/compare-version-numbers/submissions/1780076236/

Given two version strings, version1 and version2, compare them. A version string consists of revisions separated by dots '.'. The value of the revision is its integer conversion ignoring leading zeros. To compare version strings, compare their revision values in left-to-right order. If one of the version strings has fewer revisions, treat the missing revision values as 0. Return the following: If version1 < version2, return -1. If version1 > version2, return 1. Otherwise, return 0.

```java
            int num2 = (i < v2.length)? Integer.parseInt(v2[i]) : 0;

            if(num1 < num2){
                return -1;
            }else if(num1 > num2){
                return 1;
            }
        }

        return 0;
        
    }

        int n = Math.max(v1.length, v2.length);

        for(int i =0; i<n; i++){
            int num1 = (i < v1.length)? Integer.parseInt(v1[i]) : 0;
```
