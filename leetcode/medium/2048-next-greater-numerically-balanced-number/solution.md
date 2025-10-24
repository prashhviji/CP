# 2048. Next Greater Numerically Balanced Number

**Link:** https://leetcode.com/problems/next-greater-numerically-balanced-number/submissions/1809978895/

An integer x is numerically balanced if for every digit d in the number x, there are exactly d occurrences of that digit in x. Given an integer n, return the smallest numerically balanced number strictly greater than n.

```java
        while(x>0){
            count[x%10]++;
            x/=10;
        }

        int[] count=new int[10];

    }
    private boolean isBalance(int x){
        return -1;
        for(int d=0; d<10; d++){
            if(count[d]>0 && count[d] != d){
                return false;
            }
        }
        }
            }
                return i;
```
