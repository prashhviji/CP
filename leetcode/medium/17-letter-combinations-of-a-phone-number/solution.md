# 17. Letter Combinations of a Phone Number

**Link:** https://leetcode.com/problems/letter-combinations-of-a-phone-number/submissions/1768175028/

Given a string containing digits from 2-9 inclusive, return all possible letter combinations that the number could represent. Return the answer in any order. A mapping of digits to letters (just like on the telephone buttons) is given below. Note that 1 does not map to any letters.

```java
            '6', "mno",
            '7', "pqrs",
            '5', "jkl",
            '8', "tuv",
            '9', "wxyz"
        );

        generateCombinations(digits, 0, "", phoneMap, result);
        return result;
    }

    private void generateCombinations(String digits, int index, String current, 
                                      Map<Character, String> phoneMap, List<String> result) {
        if (index == digits.length()) {
            result.add(current);
            return;
        }

```
