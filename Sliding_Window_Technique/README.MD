## 🪟 Sliding Window Technique
### What is Sliding Window ?
<p>
  The name itself suggests what it is. There is a sequence of given length in which we consider a particular segment( window ) to perform certain operation. If we get required result from current segment( window ) then our work is done, if not then we move our segment( window ) furthur till we reach the end.<br>
  By sliding it mean that we are just pushing that window furthur into the sequence and not repeatedly calculating results again and again.<br>
  We can have linear time complexity O(n) with this technique.
  Still not understood? Here's a visual demo,
</p>
<div align="center">
  <img src="https://raw.githubusercontent.com/someshvk/DSA_Patterns/main/Sliding_Window_Technique/images/Sliding-window-technique.jpg" alt="sliding_window" />
</div>

##
### Types of Sliding Window
<p>
  There are two types of sliding window:<br>
  <b>1. Fixed sized -></b><br>
  In this type, the window size is fixed to a particular number. You move the window throughout the sequence without changing the window size.
  <div align="center">
    <img src="https://raw.githubusercontent.com/someshvk/DSA_Patterns/main/Sliding_Window_Technique/images/fixed_window.gif" alt="fixed_window" />
  </div><br>
  <b>1. Variable sized -></b><br>
  In this type, the window size is variable. You move the window throughout the sequence and the window size changes according to the type of operation we perform. You can imagine a caterpillar 🐛 moving around a branch.<br>
  <div align="center">
    <img src="https://raw.githubusercontent.com/someshvk/DSA_Patterns/main/Sliding_Window_Technique/images/variable_window.gif" alt="variable_window" />
  </div>
</p>

##
### How to identify?
<p>You can identify this pattern by checking following points,</p>
<ol>
  <li>The given problem is on a linear data structure like Arrays, Strings or a Linked Lists.</li>
  <li>When asked to find Subarrays, Substrings or a contiguous sunsequence.</li>
  <li>When asked to calculate Minimum, Maximum, Longest, Shortest or Contained value within a sequence.</li>
  <li>When asked something like k-distinct, k elements,...</li>
</ol>

##
### How to solve?
<p>
  Consider that you have to find the maximum sum subarray of size <b>k</b> from the given array.<br>
  <b>array = [4, 2, 1 ,7, 8, 1]</b><br>
  <b>k = 3</b><br><br>
  So to find the max subarray, we will consider a window of size 3 and initially our window would be,<br>
  window = [4, 2, 1]<br><br>
  And the sum of our window is,<br>
  sum = 4+2+1 = 7<br><br>
  Now we slide our window furthur and to do that we will remove the first item of window( 4 here ) and add the next item( 7 here ) to our window. So our new window would be,<br>
  window = [2, 1, 7]<br>
  sum = 10<br><br>
  <b>NOTE:</b> We removed first item and added next item here because we want to avoid repeated calculation of the window sum which we already did.<br><br>
  We repeat the same process till the end of array, and at the end our window would be,<br>
  window = [7, 8, 1]<br>
  and maximun sum would be,<br>
  max = 16<br>
</p>

##
### What next?
If you still don't understand sliding window then I would recommend to take a look at the recources mentioned below.<br>
If you understood Sliding window completely, then it is the time to jump to questions. I have also provided answers to all questions. First solve the problem on your own, if you are finding it difficult then you can check the answers.<br>
Best Luck !

##
### Some resources for more clarity
<ol>
  <li><a href="https://www.youtube.com/watch?v=MK-NZ4hN7rs" target="_blank">Sliding Window Technique YouTube video</a></li>
  <li><a href="https://medium.com/outco/how-to-solve-sliding-window-problems-28d67601a66" target="_blank">Article on medium</a></li>
</ol>
