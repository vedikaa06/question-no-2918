# question-no-2918
Solution to the question no 2918 on leet code 

2918. Minimum Equal Sum of Two Arrays After Replacing Zeros

You are given two arrays nums1 and nums2 consisting of positive integers.

You have to replace all the 0's in both arrays with strictly positive integers such that the sum of elements of both arrays becomes equal.

Return the minimum equal sum you can obtain, or -1 if it is impossible.

Solution Overview:
Compute Initial Sums:

For each array, sum all elements.

For every 0, assume the minimum valid replacement (1) to get the minimum possible sum.

Check for Impossibility:

If one array has no zeros, its sum is fixed.

If the other array has zeros but still can't reach the fixed sum, it's impossible → return -1.

Return the Minimum Equal Sum:

If possible, return the maximum of the two (possibly adjusted) sums — the smallest value they both can reach.

Key Insight:
Zeros give flexibility. But if one array has no zeros, it cannot increase its sum.

So if the other array can’t match that fixed sum using only 1s for its zeros, the task is impossible.

Let me know if you want this turned into comments in the code.
