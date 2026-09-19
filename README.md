# Week 4 Assignment

Java implementations for five array and subarray algorithm problems.

## Problems

### A1. Product of Array Except Self

`A1_ProductOfArrayExceptSelf/ProductOfArrayExceptSelf.java`

Uses a forward pass for products to the left and a backward pass for products
to the right. It does not use division and runs in `O(n)` time with `O(1)`
extra space beyond the output array.

### A2. Maximum Subarray

`A2_MaximumSubarray/MaximumSubarray.java`

Uses Kadane's algorithm to find the largest sum of a non-empty contiguous
subarray in `O(n)` time and `O(1)` extra space.

### A3. 3Sum

`A3_3Sum/ThreeSum.java`

Sorts the input and uses two pointers to find all unique zero-sum triplets in
`O(n^2)` time.

### A4. Subarray Sum Equals K

`A4_SubarraySumEqualsK/SubarraySumEqualsK.java`

Uses prefix-sum frequencies in a hash map to count subarrays with sum `k` in
`O(n)` time and `O(n)` space.

### A5. Find Minimum in Rotated Sorted Array

`A5_FindMinimumInRotatedSortedArray/FindMinimumInRotatedSortedArray.java`

Uses modified binary search to find the minimum in `O(log n)` time.

## Compile and Run

Each folder includes the Java source file and its compiled `.class` file.
From the repository root, compile all solutions:

```powershell
Get-ChildItem -Recurse -Filter *.java | ForEach-Object { javac $_.FullName }
```

Run an individual solution from its folder:

```powershell
java ProductOfArrayExceptSelf
java MaximumSubarray
java ThreeSum
java SubarraySumEqualsK
java FindMinimumInRotatedSortedArray
```

Each `main` method runs the sample cases from the assignment.
