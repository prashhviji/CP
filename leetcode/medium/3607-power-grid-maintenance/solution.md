# 3607. Power Grid Maintenance

**Link:** https://leetcode.com/problems/power-grid-maintenance/submissions/1822571680/

You are given an integer c representing c power stations, each with a unique identifier id from 1 to c (1‑based indexing). These stations are interconnected via n bidirectional cables, represented by a 2D array connections, where each element connections[i] = [ui, vi] indicates a connection between station ui and station vi. Stations that are directly or indirectly connected form a power grid. Initially, all stations are online (operational). You are also given a 2D array queries, where each query is one of the following two types: [1, x]: A maintenance check is requested for station x. If station x is online, it resolves the check by itself. If station x is offline, the check is resolved by the operational station with the smallest id in the same power grid as x. If no operational station exists in that grid, return -1. [2, x]: Station x goes offline (i.e., it becomes non-operational). Return an array of integers representing the results of each query of type [1, x] in the order they appear.

```java
                } else {
                    online[x] = true;
                    if (station == -1 || station > x) {
                        minimumOnlineStations.put(root, x);
                    }
                }
            }
        }

        Collections.reverse(ans);
        return ans.stream().mapToInt(Integer::intValue).toArray();
    }
}
```
