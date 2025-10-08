# 853. Car Fleet

**Link:** https://leetcode.com/problems/car-fleet/

There are n cars at given miles away from the starting mile 0, traveling to reach the mile target. You are given two integer arrays position and speed, both of length n, where position[i] is the starting mile of the ith car and speed[i] is the speed of the ith car in miles per hour. A car cannot pass another car, but it can catch up and then travel next to it at the speed of the slower car. A car fleet is a single car or a group of cars driving next to each other. The speed of the car fleet is the minimum speed of any car in the fleet. If a car catches up to a car fleet at the mile target, it will still be considered as part of the car fleet. Return the number of car fleets that will arrive at the destination.

```java
        for (int[] car : cars) {
            int pos = car[0];
            int spd = car[1];
        
        Stack<Double> stack = new Stack<>();
            double timeTaken = (double)(target - pos) / spd;
            
            if (stack.isEmpty() || timeTaken > stack.peek()) {
                stack.push(timeTaken);
            }
        }
        
        return stack.size();       
    }
}
        
        Arrays.sort(cars, (a, b) -> Integer.compare(b[0], a[0]));
```
