# karat-interview
karat-interview

******************************
Knowledge based questions:

System Internals (Memory / CPU)
1. Thread v/s Process. How does one thread communicates with other thread, and how does one process communicate with other process?
1. What is garbage collection? What needs to be done if it is not handled by the programming language? Under which scenarios garbage collection does not work well?
1. Stack v/s Heap in the context of memory allocation, variables etc.
1. A couple of other questions / followups that I don't remember.

OOD
1. Dependency Injection
1. Inheritance v/s Composition
1. One more question I don't recall (not polymorphism).

Coding Questions:

1. Given a string and an array of words, find the first word that can be created by using letters of the string. For eg. if string is "balloons" and words are ["son", "ball", "friends"] return "son" as it is the first word that can be constructed using letters from "balloons".
2. https://leetcode.com/problems/word-search/ but have to also return position of where the word was found in the matrix and need to go only in right and down directions in the matrix. Word is guaranteed to be in the matrix.
3. Multiple words are given for searching in the word search problem (2) but each letter in the matrix can only be used towards one word. Not completely sure if the objective was trying to match maximum words or returning the index of matching words (assuming all can be matched). Very few minutes were left for this so couldn't discuss much with the interviewer about this. I think I only provided some brute force solution but not sure if it was correct.


******************************

|S.No |Interview Question |Number of times candidates experienced this question in interviews|
|--|--|---|
|1| [Text Justification LeetCode Solution](https://tutorialcup.com/leetcode-solutions/text-justification.htm) | 7785|
|2| [Count subarrays with equal number of 1’s and 0’s](https://tutorialcup.com/interview/hashing/count-subarrays-with-equal-number-of-1s-and-0s.htm) | 5265|
|3| [Employee Free Time LeetCode Solution](https://tutorialcup.com/leetcode-solutions/employee-free-time-leetcode-solution.htm) | 4587|
|4| [Length of the largest subarray with contiguous elements](https://tutorialcup.com/interview/hashing/length-of-the-largest-subarray-with-contiguous-elements.htm) | 4063|
|5| [Maximum Length of Repeated Subarray](https://tutorialcup.com/interview/array/maximum-length-of-repeated-subarray.htm) | 3450|
|6| [BFS for Disconnected Graph](https://tutorialcup.com/interview/graph/bfs-for-disconnected-graph.htm) | 2918|
|7| [Generate all possible sorted arrays from alternate elements of two given sorted arrays](https://tutorialcup.com/interview/array/generate-all-possible-sorted-arrays-from-alternate-elements-of-two-given-sorted-arrays.htm) | 2864|
|8| [Lowest Common Ancestor of a Binary Tree Leetcode Solution](https://tutorialcup.com/leetcode-solutions/lowest-common-ancestor-of-a-binary-tree-leetcode-solution.htm) | 2719|
|9| [Maximize sum of consecutive differences in a circular array](https://tutorialcup.com/interview/array/maximize-sum-of-consecutive-differences-in-a-circular-array.htm) | 2563|

******************************

Find the top left and bottom right coordinates of a rectangle of 0's within a matrix of 1's. It's essentially a modified version of the finding the number of island problem where you only need to dfs to the right and down.
Ex.
[[ 1, 1, 1, 1],
[ 1, 0, 0, 1],
[ 1, 0, 0, 1],
[ 1, 1, 1, 1]]
Expected output: [[1,1], [2,2]]

Follow up question: Expand it so it works for any number of rectangles. I ran out of time to code this part so get throught the first part quickly. Main part of this problem is updating how results are stored and tracking what's been seen.
Ex.
[[0, 1, 1, 1],
[1, 0, 0, 1],
[1, 0, 0, 1],
[1, 1, 1, 1]]
Expected output: [ [[0,0],[0,0]], [[1,1], [2,2]] ]

https://leetcode.com/problems/number-of-islands

******************************

Knowledge based questions:

user mode vs kernel mode
2)what is context switching? and what are triggers for context switchin?
3)overloading vs overriding
4)a code snippet on abstarct class vs derived class about initilaizing a new object.
another code snippet based question, to identify issues in program.
what is swap space?
Coding questions

question 1 - Minin game same as https://leetcode.com/discuss/interview-question/1740425/indeed-phone-interview-mini-game
```
question 2 -> a dfs based graph(grid) question

While your players are waiting for a game, you've developed a solitaire game for the players to pass the time with.
The player is given an NxM board of tiles from 0 to 9 like this:

4 4 4 4
5 5 5 4
2 5 7 5
The player selects one of these tiles, and that tile will disappear, along with any tiles with the same number that are connected with that tile (up, down, left, or right), and any tiles with the same number connected with those, and so on. For example, if the 4 in the upper left corner is selected, these five tiles disappear

4< >4< >4< >4<
5 5 5 >4<
2 5 7 5
If the 5 just below it is selected, these four tiles disappear. Note that tiles are not connected diagonally.
4 4 4 4
5< >5< >5< 4
2 >5< 7 5
Write a function that, given a grid of tiles and a selected row and column of a tile, returns how many tiles will disappear.

grid1 = [[4, 4, 4, 4],
        [5, 5, 5, 4],
        [2, 5, 7, 5]]
        
disappear(grid1, 0, 0) => 5
disappear(grid1, 1, 1) => 4
disappear(grid1, 1, 0) => 4
This is the grid from above.

Additional Inputs
grid2 = [[0, 3, 3, 3, 3, 3, 3],
[0, 1, 1, 1, 1, 1, 3],
[0, 2, 2, 0, 2, 1, 4],
[0, 1, 2, 2, 2, 1, 3],
[0, 1, 1, 1, 1, 1, 3],
[0, 0, 0, 0, 0, 0, 0]]

grid3 = [[0]]

grid4 = [[1, 1, 1],
[1, 1, 1],
[1, 1, 1]]

All Test Cases
disappear(grid1, 0, 0) => 5
disappear(grid1, 1, 1) => 4
disappear(grid1, 1, 0) => 4
disappear(grid2, 0, 0) => 12
disappear(grid2, 3, 0) => 12
disappear(grid2, 1, 1) => 13
disappear(grid2, 2, 2) => 6
disappear(grid2, 0, 3) => 7
disappear(grid3, 0, 0) => 1
disappear(grid4, 0, 0) => 9

N - Width of the grid
M - Height of the grid
```

******************************


