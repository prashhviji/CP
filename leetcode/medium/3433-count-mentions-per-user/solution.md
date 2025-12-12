# 3433. Count Mentions Per User

**Link:** https://leetcode.com/problems/count-mentions-per-user/description/

You are given an integer numberOfUsers representing the total number of users and an array events of size n x 3. Each events[i] can be either of the following two types: Message Event: ["MESSAGE", "timestampi", "mentions_stringi"] This event indicates that a set of users was mentioned in a message at timestampi. The mentions_stringi string can contain one of the following tokens: id<number>: where <number> is an integer in range [0,numberOfUsers - 1]. There can be multiple ids separated by a single whitespace and may contain duplicates. This can mention even the offline users. ALL: mentions all users. HERE: mentions all online users. Offline Event: ["OFFLINE", "timestampi", "idi"] This event indicates that the user idi had become offline at timestampi for 60 time units. The user will automatically be online again at time timestampi + 60. Return an array mentions where mentions[i] represents the number of mentions the user with id i has across all MESSAGE events. All users are initially online, and if a user goes offline or comes back online, their status change is processed before handling any message event that occurs at the same timestamp. Note that a user can be mentioned multiple times in a single message event, and each mention should be counted separately.

```java
            } else if (event.get(0).equals("OFFLINE")) {
                handleMessage(event, mentions, offlineTime);
            if (event.get(0).equals("MESSAGE")) {
        for (List<String> event : events) {

        });
(0)) : timeA - timeB;
            int timeB = Integer.parseInt(b.get(1));
            return timeA == timeB ? b.get(0).compareTo(a.get
        events.sort((a, b) -> {
            int timeA = Integer.parseInt(a.get(1));

        int[] offlineTime = new int[numberOfUsers];
        int[] mentions = new int[numberOfUsers];
List<List<String>> events) {
    public int[] countMentions(int numberOfUsers, 
class Solution {
```
