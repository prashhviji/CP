# 653. Two Sum IV - Input is a BST

**Link:** https://leetcode.com/problems/two-sum-iv-input-is-a-bst/submissions/1834522112/

Given the root of a binary search tree and an integer k, return true if there exist two elements in the BST such that their sum is equal to k, or false otherwise.

```java
        inorder(root, nums);
        int left = 0;
        int right = nums.size()-1;
        while(left < right){
            int sum =  nums.get(left) + nums.get(right);
            if(sum == k) return true;
            else if(sum < k) left++;
            else right --;
        }
        return false;
    }

    private void inorder(TreeNode node, List<Integer> list){
        if(node == null) return;
        inorder(node.left, list);
        list.add(node.val);
        inorder(node.right, list);
    }
```
