# LockerRoomProject
Problem:
There are n lockers in a hallway numbered sequentially from 1 to n. Initially, all the locker doors are closed.  You make n passes by the lockers, each time starting with locker #1. On the ith pass, i = 1, 2, ..., n, you toggle the door of every ith locker. If the door is closed, you open it, if it is open, you close it. For example, after the first pass every door is open. On the second pass you only toggle the even-numbered lockers (#2, #4, ...) so that after the second pass the even doors are closed and the odd ones are opened. The third time through you close the door of locker #3 (opened from the first pass), open the door of locker #6 (closed from the second pass), and so on.  After the last pass, which locker doors are open and which are closed?

Version 1:
To understand the outcome of the problem, I simulate the doors open and closing by running a double loop. The outcome showed me that only the lockers with a perfect square are open and the rest are closed. Knowing this, I created a more efficient code and applied it in Version 2.

Version 2:
To improve efficiency, I created a function that checks whether the locker is a perfect square using binary search. This method vastly brought down the runtime, which is shown using the chrono library.
