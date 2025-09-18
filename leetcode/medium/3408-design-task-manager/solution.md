# 3408. Design Task Manager

**Link:** https://leetcode.com/problems/design-task-manager/submissions/1774748576/

There is a task management system that allows users to manage their tasks, each associated with a priority. The system should efficiently handle adding, modifying, executing, and removing tasks. Implement the TaskManager class: TaskManager(vector<vector<int>>& tasks) initializes the task manager with a list of user-task-priority triples. Each element in the input list is of the form [userId, taskId, priority], which adds a task to the specified user with the given priority. void add(int userId, int taskId, int priority) adds a task with the specified taskId and priority to the user with userId. It is guaranteed that taskId does not exist in the system. void edit(int taskId, int newPriority) updates the priority of the existing taskId to newPriority. It is guaranteed that taskId exists in the system. void rmv(int taskId) removes the task identified by taskId from the system. It is guaranteed that taskId exists in the system. int execTop() executes the task with the highest priority across all users. If there are multiple tasks with the same highest priority, execute the one with the highest taskId. After executing, the taskId is removed from the system. Return the userId associated with the executed task. If no tasks are available, return -1. Note that a user may be assigned multiple tasks.

```java
    public void add(int userId, int taskId, int priority) {
        pq.add(new int[]{priority, taskId});

    }
        taskOwner = new HashMap<>();
        for (List<Integer> t : tasks) add(t.get(0), t.get(1), t.get(2));
        taskPriority = new HashMap<>();
        });
            return b[1] - a[1];
            if (b[0] != a[0]) return b[0] - a[0];
        pq = new PriorityQueue<>((a,b) -> {
    public TaskManager(List<List<Integer>> tasks) {

    private Map<Integer,Integer> taskOwner;
    private Map<Integer,Integer> taskPriority;
    private PriorityQueue<int[]> pq;
class TaskManager {
```
