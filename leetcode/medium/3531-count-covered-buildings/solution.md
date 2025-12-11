# 3531. Count Covered Buildings

**Link:** https://leetcode.com/problems/count-covered-buildings/submissions/1853096788/

You are given a positive integer n, representing an n x n city. You are also given a 2D grid buildings, where buildings[i] = [x, y] denotes a unique building located at coordinates [x, y]. A building is covered if there is at least one building in all four directions: left, right, above, and below. Return the number of covered buildings.

```java
            TreeSet<Integer> cols = rowToCol.get(x);
            TreeSet<Integer> rows = colToRow.get(y);
            
            Integer left = cols.lower(y);
            Integer right = cols.higher(y);
            Integer up = rows.lower(x);
            Integer down = rows.higher(x);
            
            if ((left != null) && (right != null) && (up != null) && (down != null)) {
                cnt++;
            }
        }
        return cnt;
    }
}


```
