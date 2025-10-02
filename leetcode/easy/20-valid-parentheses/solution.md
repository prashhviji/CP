# 20. Valid Parentheses

**Link:** https://leetcode.com/problems/valid-parentheses/submissions/1788852962/

Given a string s containing just the characters '(', ')', '{', '}', '[' and ']', determine if the input string is valid. An input string is valid if: Open brackets must be closed by the same type of brackets. Open brackets must be closed in the correct order. Every close bracket has a corresponding open bracket of the same type.

```java
            if(mapping.containsValue(c)){
        }
                stack.push(c);
            }else if(mapping.containsKey(c)){
                if(stack.isEmpty() || mapping.get(c) != stack.pop()){
            }
                    return false;
                }
        mapping.put(']', '[');

        for(char c : s.toCharArray()){
        mapping.put('}', '{');
        return stack.isEmpty();

        

    }
}
```
