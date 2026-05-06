# leetcode-solutions
Solved LeetCode DSA problems using Java with optimized approaches and clean code.
# 217. Contains Duplicate

| Field | Value |
|---|---|
| Difficulty | Easy |
| Tags | Array, Hash Table |

## Problem
Given an integer array nums, return true if any value appears at least twice in the array, and return false if every element is distinct.

## Java Solution

```java
class Solution {
    public boolean containsDuplicate(int[] nums) {

        HashSet<Integer> set = new HashSet<>();

        for (int num : nums) {

            if (set.contains(num)) {
                return true;
            }

            set.add(num);
        }

        return false;
    }
}
