# 230. Kth Smallest Element in a BST

**Link:** https://leetcode.com/problems/kth-smallest-element-in-a-bst/

Given the root of a binary search tree, and an integer k, return the kth smallest value (1-indexed) of all the values of the nodes in the tree.

```java
    private int result = 0;
    public int kthSmallest(TreeNode root, int k) {
        inorder(root, k);
        return result;
    }
    private void inorder(TreeNode node, int k){
        if(node == null) return;
        inorder(node.left,k);
        count ++;
        if(count == k){
            result = node.val;
            return;
        }
        inorder(node.right,k);
    }
}
    private int count = 0;
```
