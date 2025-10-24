# 106. Construct Binary Tree from Inorder and Postorder Traversal

**Link:** https://leetcode.com/problems/construct-binary-tree-from-inorder-and-postorder-traversal/submissions/1810175211/

Given two integer arrays inorder and postorder where inorder is the inorder traversal of a binary tree and postorder is the postorder traversal of the same tree, construct and return the binary tree.

```java

    public TreeNode buildTree(int[] inorder, int[] postorder) {
        postIndex = postorder.length - 1;


    private HashMap<Integer, Integer> inorderIndexMap = new HashMap<>();
        for (int i = 0; i < inorder.length; i++) {
            inorderIndexMap.put(inorder[i], i);
        }

        return buildSubtree(postorder, 0, inorder.length - 1);
    }

    private TreeNode buildSubtree(int[] postorder, int left, int right) {
        if (left > right) {
            return null;
        }

```
