# 144. Binary Tree Preorder Traversal

**Link:** https://leetcode.com/problems/binary-tree-preorder-traversal/

Given the root of a binary tree, return the preorder traversal of its nodes' values.

```java
        List<Integer> res = new ArrayList<>();
        helper(root,res);
        return res;
    }
    
    public void helper(TreeNode root, List<Integer> res){
        if(root != null){
            res.add(root.val);
            helper(root.left , res);
            helper(root.right, res);
        }
    }
}
```
