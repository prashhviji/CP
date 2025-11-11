# 1008. Construct Binary Search Tree from Preorder Traversal

**Link:** https://leetcode.com/problems/construct-binary-search-tree-from-preorder-traversal/submissions/1826663923/

Given an array of integers preorder, which represents the preorder traversal of a BST (i.e., binary search tree), construct the tree and return its root. It is guaranteed that there is always possible to find a binary search tree with the given requirements for the given test cases. A binary search tree is a binary tree where for every node, any descendant of Node.left has a value strictly less than Node.val, and any descendant of Node.right has a value strictly greater than Node.val. A preorder traversal of a binary tree displays the value of the node first, then traverses Node.left, then traverses Node.right.

```java
class Solution {
    public TreeNode bstFromPreorder(int[] preorder) {
 */
        return helper(preorder, 0, preorder.length - 1);
    }

    private TreeNode helper(int[] preorder, int start, int end){
        if(start > end){
            return null;
        }

        int i;
        TreeNode node = new TreeNode(preorder[start]);
        for( i = start + 1; i <= end; i++){
            if(preorder[i] > node.val){
                break;
            }
```
