# 79. Word Search

**Link:** https://leetcode.com/problems/word-search/submissions/1766466114/

Given an m x n grid of characters board and a string word, return true if word exists in the grid. The word can be constructed from letters of sequentially adjacent cells, where adjacent cells are horizontally or vertically neighboring. The same letter cell may not be used more than once.

```java
        char temp = board[i][j]; 
        board[i][j] = '*'; 

        boolean found = search(board, word, i + 1, j, k + 1) ||
                        search(board, word, i - 1, j, k + 1) ||
                        search(board, word, i, j + 1, k + 1) ||
                        search(board, word, i, j - 1, k + 1);

        board[i][j] = temp; 

        if (i < 0 || j < 0 || i >= board.length || j >= board[0].length 
            || board[i][j] != word.charAt(k)) return false;
        if (k == word.length()) return true;

    private boolean search(char[][] board, String word, int i, int j, int k) {
    }
        return false;
```
