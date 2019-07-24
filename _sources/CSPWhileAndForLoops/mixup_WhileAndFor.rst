..   qnum::
  :start: 1
  :prefix: 8-8-

Mixed Up Code Practice
------------------------------

.. parsonsprob:: ch8ex1muc
   :numbered: left
   :adaptive:

   The following program segment should display the value of n as long as n is less than 5. But the blocks have been mixed up and include an extra block that isn't needed in the solution.
   -----
   n <- 0
   =====
   while n < 5:
   =====
       DISPLAY(n)
   =====
       n = n + 1
   =====
   while n > 5: #distractor