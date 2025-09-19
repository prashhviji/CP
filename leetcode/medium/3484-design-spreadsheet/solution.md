# 3484. Design Spreadsheet

**Link:** https://leetcode.com/problems/design-spreadsheet/submissions/1775689496/

A spreadsheet is a grid with 26 columns (labeled from 'A' to 'Z') and a given number of rows. Each cell in the spreadsheet can hold an integer value between 0 and 105. Implement the Spreadsheet class: Spreadsheet(int rows) Initializes a spreadsheet with 26 columns (labeled 'A' to 'Z') and the specified number of rows. All cells are initially set to 0. void setCell(String cell, int value) Sets the value of the specified cell. The cell reference is provided in the format "AX" (e.g., "A1", "B10"), where the letter represents the column (from 'A' to 'Z') and the number represents a 1-indexed row. void resetCell(String cell) Resets the specified cell to 0. int getValue(String formula) Evaluates a formula of the form "=X+Y", where X and Y are either cell references or non-negative integers, and returns the computed sum.

```java
    public int getValue(String formula) {
    
    }
        String arr[] = formula.substring(1).split("\\+");
        return getCell(arr[0]) + getCell(arr[1]);
    }
 
    public int getCell(String cell) {
        if(cell.charAt(0)>='0' && cell.charAt(0)<='9') {
            return Integer.parseInt(cell);
        }
        else return map.getOrDefault(cell,0);
    }
}

        map.put(cell, 0);
    public void resetCell(String cell) {
    
```

## Mistake Analysis

TAGS: Syntax Error, Data Structure, Logic Error

1. **Key Issues**: Attempt 1 has numerous syntax errors (missing semicolons, incorrect class definition).  The `HashMap` is declared but not properly initialized within the constructor.  No cell value retrieval logic is implemented. The `setCell` method lacks the essential parsing of the cell string to extract column and row indices.

2. **Evolution**: No evolution is shown as only a single incomplete attempt is provided.  The code lacks basic functionality and proper structure.

