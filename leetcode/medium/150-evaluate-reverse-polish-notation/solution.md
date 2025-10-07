# 150. Evaluate Reverse Polish Notation

**Link:** https://leetcode.com/problems/evaluate-reverse-polish-notation/submissions/1793760522/

You are given an array of strings tokens that represents an arithmetic expression in a Reverse Polish Notation. Evaluate the expression. Return an integer that represents the value of the expression. Note that: The valid operators are '+', '-', '*', and '/'. Each operand may be an integer or another expression. The division between two integers always truncates toward zero. There will not be any division by zero. The input represents a valid arithmetic expression in a reverse polish notation. The answer and all the intermediate calculations can be represented in a 32-bit integer.

```java
            }else if(c.equals("*")){
                stack.push(stack.pop() * stack.pop());
            }else if(c.equals("/")){
                int second = stack.pop();
            }else{
                int first = stack.pop();
                stack.push(first / second);
                stack.push(first - second);
                int second = stack.pop();
                int first = stack.pop();
                stack.push(stack.pop() + stack.pop());
            }else if(c.equals("-")){
        for(String c : tokens){
            if(c.equals("+")){
                stack.push(Integer.parseInt(c));
            }
        }
```
