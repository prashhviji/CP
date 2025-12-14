# 199. Binary Tree Right Side View

**Link:** https://leetcode.com/problems/binary-tree-right-side-view/submissions/1855607457/

Given the root of a binary tree, imagine yourself standing on the right side of it, return the values of the nodes you can see ordered from top to bottom.

```java
    public List<Integer> rightSideView(TreeNode root) {
        List<Integer> result = new ArrayList<Integer>();
    }

    private void rightSideView(TreeNode node, List<Integer> result, int Depth){
        if(node == null) return;

        if(Depth == result.size()){
            result.add(node.val);
        }

        rightSideView(node.right, result, Depth + 1);
        rightSideView(node.left, result, Depth + 1);
        rightSideView(root , result , 0);
        return result;
    }
}
```
