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
### Some resources for more clarity
<ol>
  <li><a href="https://www.youtube.com/watch?v=MK-NZ4hN7rs" target="_blank">Sliding Window Technique YouTube video</a></li>
  <li><a href="https://medium.com/outco/how-to-solve-sliding-window-problems-28d67601a66" target="_blank">Article on medium</a></li>
</ol>
