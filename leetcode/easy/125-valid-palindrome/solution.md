# 125. Valid Palindrome

**Link:** https://leetcode.com/problems/valid-palindrome/submissions/1863385046/

A phrase is a palindrome if, after converting all uppercase letters into lowercase letters and removing all non-alphanumeric characters, it reads the same forward and backward. Alphanumeric characters include letters and numbers. Given a string s, return true if it is a palindrome, or false otherwise.

```java
        int left = 0;
        int right = s.length() -1;

        while(left < right){
            if(s.charAt(left) != s.charAt(right)){
        }
                return false;
            }
    }
        return true;
            left ++;
            right --;
}
```
