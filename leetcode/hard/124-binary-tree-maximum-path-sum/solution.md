# 124. Binary Tree Maximum Path Sum

**Link:** https://leetcode.com/problems/binary-tree-maximum-path-sum/

A path in a binary tree is a sequence of nodes where each pair of adjacent nodes in the sequence has an edge connecting them. A node can only appear in the sequence at most once. Note that the path does not need to pass through the root. The path sum of a path is the sum of the node's values in the path. Given the root of a binary tree, return the maximum path sum of any non-empty path.

```java
        int[] res = { root.val };
        dfs(root, res);
        return res[0];
    }

    private int dfs(TreeNode node, int[] res){
        if(node == null) return 0;
    }
 * }
 */
class Solution {
    public int maxPathSum(TreeNode root) {
        int leftsum = Math.max(0, dfs(node.left, res));
        int rightsum = Math.max(0,dfs(node.right, res));
        res[0] = Math.max(res[0], leftsum + rightsum + node.val);
        return Math.max(leftsum, rightsum) + node.val;
}
```
