# 235. Lowest Common Ancestor of a Binary Search Tree

**Link:** https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/submissions/1845933747/

Given a binary search tree (BST), find the lowest common ancestor (LCA) node of two given nodes in the BST. According to the definition of LCA on Wikipedia: “The lowest common ancestor is defined between two nodes p and q as the lowest node in T that has both p and q as descendants (where we allow a node to be a descendant of itself).”

```java
    public TreeNode lowestCommonAncestor(TreeNode root, TreeNode p, TreeNode q) {
        while(root != null){
            if(p.val > root.val && q.val > root.val ){
                root = root.right;
            }else if(p.val < root.val && q.val < root.val){
                root = root.left;
            }else{
                return root;
            }
        }
class Solution {

 */
 * }
 *     TreeNode(int x) { val = x; }
 *     TreeNode right;
 *     TreeNode left;
```
