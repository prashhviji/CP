# 110. Balanced Binary Tree

**Link:** https://leetcode.com/problems/balanced-binary-tree/

Given a binary tree, determine if it is height-balanced.

```java

    private int depth(TreeNode node){
        if(node == null) return 0;

        int leftHeight = depth(node.left);
        int rightHeight = depth(node.right);

        if(Math.abs(leftHeight - rightHeight) > 1){
            balanced = false;
        }
        return Math.max(leftHeight, rightHeight) + 1;
    }
}
    }
```
