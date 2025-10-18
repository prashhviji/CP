# 987. Vertical Order Traversal of a Binary Tree

**Link:** https://leetcode.com/problems/vertical-order-traversal-of-a-binary-tree/submissions/1805249641/

Given the root of a binary tree, calculate the vertical order traversal of the binary tree. For each node at position (row, col), its left and right children will be at positions (row + 1, col - 1) and (row + 1, col + 1) respectively. The root of the tree is at (0, 0). The vertical order traversal of a binary tree is a list of top-to-bottom orderings for each column index starting from the leftmost column and ending on the rightmost column. There may be multiple nodes in the same row and same column. In such a case, sort these nodes by their values. Return the vertical order traversal of the binary tree.

```java
        });

        List<List<Integer>> result = new ArrayList<>();
        int prevCol = Integer.MIN_VALUE;

        // Step 3: Group by column
        for (int[] node : nodes) {
            int col = node[0], val = node[2];
            if (col != prevCol) {
                result.add(new ArrayList<>());
                prevCol = col;
            }
            result.get(result.size() - 1).add(val);
        }

        return result;
    }

```
