## 🪟 Sliding Window Technique
### What is Sliding Window ?
<p>
  The name itself suggests what it is. There is a sequence of given length in which we consider a particular segment( window ) to perform certain operation. If we get required result from current segment( window ) then our work is done, if not then we move our segment( window ) furthur till we reach the end.<br>
  By sliding it mean that we are just pushing that window furthur into the sequence and not repeatedly calculating results again and again.
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
