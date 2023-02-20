# Kadane's-Algorithm
Kadane's algorithm is a dynamic programming algorithm used to find the maximum subarray sum in an array of integers. The algorithm has a time complexity of O(n) and works by iterating over the array and keeping track of the maximum sum seen so far and the maximum sum ending at the current index. At each iteration, the maximum sum ending at the current index is either the current number or the sum of the current number and the maximum sum ending at the previous index. The maximum sum seen so far is updated if the maximum sum ending at the current index is greater than the maximum sum seen so far. By the end of the iteration, the maximum sum seen so far is the maximum subarray sum of the given array.

# How the code works
This code defines a function called **max_subarray_sum** which takes an array **arr** as input. It finds the maximum sum subarray in the given array and prints the subarray, the sum of the subarray, and the starting and ending indices of the subarray.

The function initializes three variables **max_so_far**, **max_ending_here**, **starting_index**, and **ending_index** to negative infinity and 0 respectively. It then iterates through the array using a for loop and updates **max_ending_here** and **max_so_far** at each step.

For each element of the array, the function checks if adding that element to **max_ending_here** would result in a larger sum. If it does, then it updates **max_ending_here**. Otherwise, it sets **max_ending_here** to the current element. It then checks if the new value of **max_ending_here** is greater than the current value of **max_so_far**, and updates **max_so_far** and the starting and ending indices of the subarray accordingly.

Finally, the function prints the input array, the maximum subarray, its sum, and the starting and ending indices of the subarray. The input array used in the example is **[-2, 1, -3, 4, -1, 2, 1, -5, 4]**.
