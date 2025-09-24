# 166. Fraction to Recurring Decimal

**Link:** https://leetcode.com/problems/fraction-to-recurring-decimal/submissions/1781144664/

Given two integers representing the numerator and denominator of a fraction, return the fraction in string format. If the fractional part is repeating, enclose the repeating part in parentheses. If multiple answers are possible, return any of them. It is guaranteed that the length of the answer string is less than 104 for all the given inputs.

```java
                result.append(")"); 
                break;
            }

            seen.put(remainder, result.length());

            remainder *= 10;
            result.append(remainder / den);
            remainder %= den; 
        }

        return result.toString();
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Data Structure

1. **Key Issues**: Attempt 1 incorrectly placed the decimal point and the loop's termination condition. Attempts 2 and 3 missed handling the decimal part after the integer part. The `unordered_map` in all attempts is correctly used to detect repeating decimals, but its usage needs to be corrected for placing the parentheses.


2. **Evolution**: Attempts moved the decimal point placement and loop logic from incorrect positions.  Attempt 3 added sign handling but remains incomplete regarding the decimal and repeating part.  The core logic of using a hashmap to find repeating sequences remained consistent but needed refinement in all attempts.

