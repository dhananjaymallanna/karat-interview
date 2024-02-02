Attempt #1 (I didn't do well in coding section)
System Design (20 mins)
Consistency: 3 scenarios to identify whether eventual consistency or strong consistency will be better. Don't remember the scenarios
Denormalization: 2 database and facebook kind of app. Want to show the number of mutual friends an author and viewer has alongside each post made. The data about it could either be computed from those 2 DBs everytime or it can be computed once and stored while denormalizing. (Mutual friends/friends part I don't remember but it was something like this)
Load Balancing: A shared doc editor (say google doc) was implemented using Round Robin Load Balacing. What's the problem in this and how to improve the app/editor
Scaling: Showed a pipeline with 6 stages each having a specific role/functionality and each of them having upper limit of number of sub-process/jobs it could perform at any given time. The entire process is considered complete when all the stages complete. Was asked to figure out the bottleneck (ans: the one with least threshold) and how to overcome it (ans: vertically scale that stage to match the threshold of the next best stage or vertically scale all the low threshold stages)
There was one more which I don't remember
Coding (30 mins)
Coding problem - https://leetcode.com/problems/check-if-every-row-and-column-contains-all-numbers/
Interviewer had a hard time understanding and eventually I ran out of time
Attempt #2 (I did well)
System Design (20 mins)
Same as in this post which is from some other user - https://leetcode.com/discuss/interview-question/1770052/Wayfair-or-Phone-or-Karat-System-Design-Questions

Coding (30 mins)
Coding problems:

https://leetcode.com/problems/subdomain-visit-count/ [Solution]
Longest common substring [Solution with test case]
Completed the 1st one while I coded 90%, including the main logic, of the 2nd one and I made sure at the begining to let the interviewer that it is dynamic programming solution/approach.

Result
Got invitation for onsite rounds
Tips
20mins and 30mins are time-boxed for each of the sections. Time doesn't roll over to coding section if you finish the system design section rapidly
Interviewer will be asking you the time & space complexities. So, be prepared for it too.
