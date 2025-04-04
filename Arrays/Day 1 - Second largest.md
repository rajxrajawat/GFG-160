# 🚀 _Day 1. Second Largest_ 🧠

The problem can be found at the following link: [Problem Link](https://www.geeksforgeeks.org/batch/gfg-160-problems/track/arrays-gfg-160/problem/second-largest3735)

## 💡 **Problem Description:**

Given an array of positive integers `arr[]`, return the second largest element from the array. If the second largest element doesn't exist, return `-1`.

**Note:** The second largest element should not be equal to the largest element.

## Code (Java)
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
