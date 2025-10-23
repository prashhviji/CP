# 100. Same Tree

**Link:** https://leetcode.com/problems/same-tree/submissions/1809503793/

Given the roots of two binary trees p and q, write a function to check if they are the same or not. Two binary trees are considered the same if they are structurally identical, and the nodes have the same value.

```java
 * }
 */
class Solution {
    public boolean isSameTree(TreeNode p, TreeNode q) {
        if(p == null && q == null){
            return true;
        }

        if(p != null && q != null && p.val == q.val){
            return isSameTree(p.left, q.left) && isSameTree(p.right, q.right);
        }
    }
        return false;
}
 *     }
```
