# 7. Reverse Integer

**Link:** https://leetcode.com/problems/reverse-integer/submissions/1750594674/

Given a signed 32-bit integer x, return x with its digits reversed. If reversing x causes the value to go outside the signed 32-bit integer range [-231, 231 - 1], then return 0. Assume the environment does not allow you to store 64-bit integers (signed or unsigned).

```java
            }
            if (rev < Integer.MIN_VALUE / 10 || (rev == Integer.MIN_VALUE / 10 && digit < -8)) 
{
                return 0; 
            }

            rev = rev * 10 + digit;  
        }

        return rev;
    }
}

                return 0; 
            if (rev > Integer.MAX_VALUE / 10 || (rev == Integer.MAX_VALUE / 10 && digit > 7)) {

            
```
