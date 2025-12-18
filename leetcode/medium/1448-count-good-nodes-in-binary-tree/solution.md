# 1448. Count Good Nodes in Binary Tree

**Link:** https://leetcode.com/problems/count-good-nodes-in-binary-tree/submissions/1858584438/

Given a binary tree root, a node X in the tree is named good if in the path from root to X there are no nodes with a value greater than X. Return the number of good nodes in the binary tree.

```java
            count++;
    private void helper(TreeNode node, int maxval){
        if(maxval <= node.val){
        return count;
    }
            maxval = node.val;
        }

        if(node.left != null){
            helper(node.left, maxval);
    public int goodNodes(TreeNode root) {
        helper(root, root.val);
 */
class Solution {
 * }
 *     }
    int count = 0;
        }
```
