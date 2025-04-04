# Day 1. Second Largest

[Problem Link](https://www.geeksforgeeks.org/batch/gfg-160-problems/track/arrays-gfg-160/problem/second-largest3735)

## **Problem Description:**

Given an array of positive integers `arr[]`, return the second largest element from the array. If the second largest element doesn't exist, return `-1`.

**Note:** The second largest element should not be equal to the largest element.
## Example
```
Input: arr[] = [12, 35, 1, 10, 34, 1]
Output: 34
Explanation: The largest element of the array is 35 and the second largest element is 34.
```
```
Input: arr[] = [10, 5, 10]
Output: 5
Explanation: The largest element of the array is 10 and the second largest element is 5.
```

## Code (Java)
```java
class Solution {
    public int getSecondLargest(int[] arr) {
        // Code Here
            int n=arr.length;
            Arrays.sort(arr);
            for(int i=n-2; i>=0; i--) {
                if(arr[i] != arr[n-1]) {
                    return arr[i];
                }
            }
        return -1;
    }
}
```
