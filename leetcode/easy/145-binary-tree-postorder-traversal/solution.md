# 145. Binary Tree Postorder Traversal

**Link:** https://leetcode.com/problems/binary-tree-postorder-traversal/submissions/1803704227/

Given the root of a binary tree, return the postorder traversal of its nodes' values.

```java
    public List<Integer> postorderTraversal(TreeNode root) {
class Solution {
 * }
 */
 *     }
 *         this.left = left;
 *         this.right = right;
 *         this.val = val;
        List<Integer> res = new ArrayList<>();
        helper(root,res);
        return res;
    }

    public void helper(TreeNode root, List<Integer> res){
        if(root != null){
            helper(root.left, res);
            helper(root.right, res);
```
