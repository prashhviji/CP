# 19. Remove Nth Node From End of List

**Link:** https://leetcode.com/problems/remove-nth-node-from-end-of-list/submissions/1750565532/

Given the head of a linked list, remove the nth node from the end of the list and return its head.

```java
            f= f.next;
        }
        if(f==null){
            return head.next;
        }
        while(f.next!=null){
            f=f.next;
            s=s.next;
        }
        s.next=s.next.next;
        return head;
    }
}
```

## Mistake Analysis

TAGS: Null Pointer, Loop Logic, Edge Cases

1. **Key Issues**: Attempt 1 is missing a closing brace and doesn't handle the case where `n` equals the list length. Attempts 2 and 3 have syntax errors. Attempt 4 fixes the syntax but has a loop logic error; `s` doesn't advance when `f` is at the second to last node.  Null pointer exceptions are possible in all attempts if not handled correctly.

2. **Evolution**: The attempts progressively improved syntax.  The core logic of using two pointers to find the node before the nth node from the end improved, but the off-by-one error and null pointer handling remained inconsistent.

