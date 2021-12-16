# Question
### Find the maximum sum subarray of size k.
### Given a positive integer k and an integer array nums, find the maximum sum subarray of size k from given array.

<p>
  <b>Example 1:</b><br>
  <b>Input :</b> nums = [ 4, 10, 2, 1 ,3, 6 ,4, 5 ] , k = 3<br>
  <b>Output :</b> Maximum sum subarray from index 0 to 2.
</p>
<p>
  <b>Example 2:</b><br>
  <b>Input :</b> nums = [ 9, 1, 50, 2 ,99, 7 ] , k = 2<br>
  <b>Output :</b> Maximum sum subarray from index 4 to 5.
</p>
<p>
  <b>Constraints :</b><br>
  <ul>
    <li>1 <= nums.length <= 10^5</li>
    <li>-10^4 <= nums[i] <= 10^4</li>
    <li>k <= nums.length </li>
  </ul>
</p>
<div>-------------------------------------------------------------------------------------------------------------------------------------------------------</div>

# Answer
<p>
  We can solve this question using Sliding window technique. We have to maintain a window of size k and whenever we slide our window through the array elements, add the upcoming element to the window and remove the leftmost element. For every window, if current sum is greater than maximum sum so far, then store current sum in max_sum_so_far variable. Repeat this till window reach the end of the array.<br>
  Following is the code in Python,
</p>

```Python
import math

# Function to find the max sum subarray of size k
def maxSumSubArray(nums: List[int], k: int):
  if k >= len(nums) or len(nums) < 1:
    return
    
  # Stores the sum of maximum sum subarray so far
  max_sum_so_far = -math.inf
  
  # Stores the sum of current window
  current_sum = 0
  
  # Stores the begining and ending index of window element
  begin = end = 0
  
  for i in range(len(nums)):
    # sum the window items
    current_sum += nums[i]
    
    # if window size is more than k
    if (i+1) >= k:
      # If current sum is greater than max sum
      if max_sum_so_far < current_sum:
        max_sum_so_far = current_sum
        end = i
      # Store first item's position of window in begin
      begin = i+1-k
      current_sum -= nums[begin]
   print("Maximum sum subarray from index ", begin, "to ", end)
```
