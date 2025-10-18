# 662. Maximum Width of Binary Tree

**Link:** https://leetcode.com/problems/maximum-width-of-binary-tree/submissions/1805319786/

Given the root of a binary tree, return the maximum width of the given tree. The maximum width of a tree is the maximum width among all levels. The width of one level is defined as the length between the end-nodes (the leftmost and rightmost non-null nodes), where the null nodes between the end-nodes that would be present in a complete binary tree extending down to that level are also counted into the length calculation. It is guaranteed that the answer will in the range of a 32-bit signed integer.

```java
        queue.add(new Pair<>(root,0));
        int maxWidth = 0;

        while(!queue.isEmpty()){
            int levelLength = queue.size();
            int levelStart = queue.peek().getValue();
            int index = 0;

            for(int i =0; i< levelLength; i++){
                Pair<TreeNode, Integer> pair = queue.poll();
        Queue<Pair<TreeNode, Integer>>queue = new LinkedList<>();
        if(root == null) return 0;
    public int widthOfBinaryTree(TreeNode root) {
class Solution {
 */
 * }
 *     }
```
