# 98. Validate Binary Search Tree

**Link:** https://leetcode.com/problems/validate-binary-search-tree/submissions/1858594081/

Given the root of a binary tree, determine if it is a valid binary search tree (BST). A valid BST is defined as follows: The left subtree of a node contains only nodes with keys strictly less than the node's key. The right subtree of a node contains only nodes with keys strictly greater than the node's key. Both the left and right subtrees must also be binary search trees.

```java
 * }
 *     }
 *     int val;
 *     TreeNode left;
 *     TreeNode right;
 *     TreeNode() {}
 *     TreeNode(int val) { this.val = val; }
 *     TreeNode(int val, TreeNode left, TreeNode right) {
 *         this.val = val;
 *         this.left = left;
 *         this.right = right;
 */
class Solution {
    public boolean isValidBST(TreeNode root) {
        return helper(root, Long.MIN_VALUE, Long.MAX_VALUE);
    }
    private boolean helper(TreeNode node, long min , long max){
        if(node == null) return true;

        if(node.val <= min || node.val >=max )return false;

        return helper(node.left , min , node.val) && helper(node.right, node.val, max);
    }
}
```
