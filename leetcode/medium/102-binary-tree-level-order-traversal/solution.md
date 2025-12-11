# 102. Binary Tree Level Order Traversal

**Link:** https://leetcode.com/problems/binary-tree-level-order-traversal/submissions/1853229492/

Given the root of a binary tree, return the level order traversal of its nodes' values. (i.e., from left to right, level by level).

```java
    private void traversalLevels(TreeNode node, int levels, List<List<Integer>>result){
        if(node == null)return;

        if(result.size() == levels){
            result.add(new ArrayList<>());
        }
        result.get(levels).add(node.val);

        traversalLevels(node.left,levels + 1, result);
        traversalLevels(node.right, levels + 1, result);
    }
}

```
