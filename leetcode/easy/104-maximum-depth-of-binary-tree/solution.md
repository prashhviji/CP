# 104. Maximum Depth of Binary Tree

**Link:** https://leetcode.com/problems/maximum-depth-of-binary-tree/description/

Given the root of a binary tree, return its maximum depth. A binary tree's maximum depth is the number of nodes along the longest path from the root node down to the farthest leaf node.

```java
 *         this.val = val;
 *         this.left = left;
 *         this.right = right;
 *     }
 * }
 */
class Solution {
    public int maxDepth(TreeNode root) {
        if(root == null)return 0;
    }

        return 1 + Math.max(maxDepth(root.left), maxDepth(root.right));
}
 *     TreeNode(int val, TreeNode left, TreeNode right) {
 *     TreeNode(int val) { this.val = val; }
```
