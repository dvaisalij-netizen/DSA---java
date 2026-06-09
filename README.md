Find Minimum and Maximum Element in an Array

Problem Statement :
Given an array of integers, find the minimum and maximum elements present in the array.

Example:
Input:
[12, 3, 15, 7, 9]
Output:
[3, 15]

Approach:
I initialized both `min` and `max` with the first element of the array. Then I traversed the remaining elements and compared each element with the current minimum and maximum values.

* If the current element was smaller than `min`, I updated `min`.
* If the current element was greater than `max`, I updated `max`.

After traversing the entire array, `min` contained the smallest element and `max` contained the largest element.

Dry Run :
Array:
[12, 3, 15, 7, 9]
Initial:
   min = 12
   max = 12

Current Element = 3
  3 < 12 → min = 3
Current Element = 15
  15 > 12 → max = 15
Current Element = 7
  No change
Current Element = 9
  No change

Final Result:
    min = 3
    max = 15
Output:
 [3, 15]
Time Complexity
 O(n)
Reason: The array is traversed only once.

Space Complexity :
 O(1)
Reason: Only two extra variables (`min` and `max`) are used.

