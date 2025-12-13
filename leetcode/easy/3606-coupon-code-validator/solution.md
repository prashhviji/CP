# 3606. Coupon Code Validator

**Link:** https://leetcode.com/problems/coupon-code-validator/submissions/1854650414/

You are given three arrays of length n that describe the properties of n coupons: code, businessLine, and isActive. The ith coupon has: code[i]: a string representing the coupon identifier. businessLine[i]: a string denoting the business category of the coupon. isActive[i]: a boolean indicating whether the coupon is currently active. A coupon is considered valid if all of the following conditions hold: code[i] is non-empty and consists only of alphanumeric characters (a-z, A-Z, 0-9) and underscores (_). businessLine[i] is one of the following four categories: "electronics", "grocery", "pharmacy", "restaurant". isActive[i] is true. Return an array of the codes of all valid coupons, sorted first by their businessLine in the order: "electronics", "grocery", "pharmacy", "restaurant", and then by code in lexicographical (ascending) order within each category.

```java
        list.addAll(liste);
        list.addAll(listg);
        list.addAll(listp);
        list.addAll(listr);
        return list;
    }
    public boolean stringCheck(String cur){
        for(char c:cur.toCharArray()){
            if(!(Character.isLetterOrDigit(c)||c=='_')){
                return false;
            }
        }
        return true;
    }
}

```
