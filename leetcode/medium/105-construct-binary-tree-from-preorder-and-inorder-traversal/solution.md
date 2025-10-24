# 105. Construct Binary Tree from Preorder and Inorder Traversal

**Link:** https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/submissions/1810166066/

Given two integer arrays preorder and inorder where preorder is the preorder traversal of a binary tree and inorder is the inorder traversal of the same tree, construct and return the binary tree.

```java

    private TreeNode build(int[] preorder, int start, int end) {
        if (start > end) return null;

        return build(preorder, 0, inorder.length - 1);        
    }

        preorderIndex = 0;
        }
        int rootVal = preorder[preorderIndex++];
        TreeNode root = new TreeNode(rootVal);
        int mid = mapping.get(rootVal);

        root.left = build(preorder, start, mid - 1);
        root.right = build(preorder, mid + 1, end);

        return root;
    }
```
