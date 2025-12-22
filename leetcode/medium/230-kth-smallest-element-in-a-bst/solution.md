# 230. Kth Smallest Element in a BST

**Link:** https://leetcode.com/problems/kth-smallest-element-in-a-bst/submissions/1862082155/

Given the root of a binary search tree, and an integer k, return the kth smallest value (1-indexed) of all the values of the nodes in the tree.

```java
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
        inorder(root, k);
    }
};
```
