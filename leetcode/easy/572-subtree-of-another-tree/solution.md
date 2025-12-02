# 572. Subtree of Another Tree

**Link:** https://leetcode.com/problems/subtree-of-another-tree/submissions/1844715303/

Given the roots of two binary trees root and subRoot, return true if there is a subtree of root with the same structure and node values of subRoot and false otherwise. A subtree of a binary tree tree is a tree that consists of a node in tree and all of this node's descendants. The tree tree could also be considered as a subtree of itself.

```java
        if(isSame(root, subRoot)) return true;
        return isSubtree(root.right, subRoot) || isSubtree(root.left, subRoot);
    }

    private boolean isSame(TreeNode a, TreeNode b){
        if(a == null && b == null)return true;
        if(a == null || b == null)return false;

        if(a.val != b.val) return false;

        return isSame(a.left, b.left) && isSame(a.right, b.right);
    }
}
        if(root == null) return false;
    public boolean isSubtree(TreeNode root, TreeNode subRoot) {
class Solution {
```
