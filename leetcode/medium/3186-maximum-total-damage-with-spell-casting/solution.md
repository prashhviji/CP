# 3186. Maximum Total Damage With Spell Casting

**Link:** https://leetcode.com/problems/maximum-total-damage-with-spell-casting/submissions/1798515529/

A magician has various spells. You are given an array power, where each element represents the damage of a spell. Multiple spells can have the same damage value. It is a known fact that if a magician decides to cast a spell with a damage of power[i], they cannot cast any spell with a damage of power[i] - 2, power[i] - 1, power[i] + 1, or power[i] + 2. Each spell can be cast only once. Return the maximum possible total damage that a magician can cast.

```java
        int n = vec.size();
        long[] f = new long[n];
        long mx = 0;
        long ans = 0;
        int j = 1;
        }
        vec.add(new int[] { -1000000000, 0 });
        for (Map.Entry<Integer, Integer> e : count.entrySet()) {
            vec.add(new int[] { e.getKey(), e.getValue() });
            count.put(p, count.getOrDefault(p, 0) + 1);
        }
        List<int[]> vec = new ArrayList<>();
    public long maximumTotalDamage(int[] power) {
        TreeMap<Integer, Integer> count = new TreeMap<>();
        for (int p : power) {
class Solution {

```
