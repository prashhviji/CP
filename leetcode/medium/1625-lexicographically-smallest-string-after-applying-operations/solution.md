# 1625. Lexicographically Smallest String After Applying Operations

**Link:** https://leetcode.com/problems/lexicographically-smallest-string-after-applying-operations/submissions/1806095730/

You are given a string s of even length consisting of digits from 0 to 9, and two integers a and b. You can apply either of the following two operations any number of times and in any order on s:

```java
                        t[p] = (char) ('0' + ((t[p] - '0' + k * a) % 10));
                    for (int p = 0; p < n; p += 2) {
                    }
                        t[p] = (char) ('0' + ((t[p] - '0' + j * a) % 10));
                    for (int p = 1; p < n; p += 2) {
                    }
                    String tStr = new String(t);
                    if (tStr.compareTo(res) < 0) {
                        res = tStr;
                    }
                }
            }
        }
        return res;
    }

    public int gcd(int num1, int num2) {
        while (num2 != 0) {
```
