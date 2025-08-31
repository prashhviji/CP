# 37. Sudoku Solver

**Link:** https://leetcode.com/problems/sudoku-solver/submissions/1754360903/

Write a program to solve a Sudoku puzzle by filling the empty cells. A sudoku solution must satisfy all of the following rules: Each of the digits 1-9 must occur exactly once in each row. Each of the digits 1-9 must occur exactly once in each column. Each of the digits 1-9 must occur exactly once in each of the 9 3x3 sub-boxes of the grid. The '.' character indicates empty cells.

```java
                    if (!sudokuSolved) removeNumber(d, row, col);
                }
            }
        } else placeNextNumbers(row, col);
    }

    public void solveSudoku(char[][] board) {
        this.board = board;
        for (int i = 0; i < N; i++)
            for (int j = 0; j < N; j++)
                if (board[i][j] != '.') placeNumber(Character.getNumericValue(board[i][j]), i, 
j);
        backtrack(0, 0);
    }
}
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Conditional Logic

1. **Key Issues**: Attempt 1 is incomplete and lacks crucial parts of a backtracking Sudoku solver.  The `placeNumber` and `removeNumber` functions aren't shown, and the logic for checking row, column, and 3x3 box constraints is missing. The recursive `backtrack` function's base case and conditional logic are unclear and incomplete.

2. **Evolution**: No evolution is shown; only a fragment of a possible attempt is provided.  Further attempts are needed for analysis.

