.. 	qnum::
	:start: 1
	:prefix: 13-7-

Mixed Up Code Practice
------------------------------

Try to solve each of the following. Click the *Check Me* button to check each solution.  You will be told if your solution is too short, has a block in the wrong order, or you are using the wrong block.  Some of the problems have an extra block that isn't needed in the correct solution.  Try to solve these on your phone or other mobile device!

.. parsonsprob:: ch13ex1muc
   :numbered: left
   :adaptive:
   :noindent:

   The program segment should print the number of temperatures that are above freezing (greater than 32 degrees). But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   temperatures <- [42,30,32,19,35,39,38]
   above_freezing <- 0
   =====
   for each item in temperatures
   =====
       if item > 32
   =====
           above_freezing <- above_freezing + 1
   =====
   DISPLAY(above_freezing)
   =====
           above_freezing <- item #distractor


.. parsonsprob:: ch13ex2muc
   :numbered: left
   :adaptive:

   The following program segment should find the maximum value of a list and display the value. But the blocks have been mixed up and include an extra block that isn't needed in the solution. But, the blocks have been mixed up and include an extra block that isn't needed in the solution. Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   max <- list[0]
   =====
   for each item in list
   =====
       if item > max
   =====
           max <- item
   =====
   DISPLAY(max)
   =====
       if item < max #distractor


.. parsonsprob:: ch13ex3muc
   :numbered: left
   :adaptive:


   The following program segment should increase the value of every item in the list by 1 if the original value is less than 3.  The shorts are originally $39.99 each. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   list <- [0,1,2,3,4]
   =====
   for each item in list
   =====
       if item < 3
   =====
           item <- item + 1
   =====
       if item > 3 #distractor


.. parsonsprob:: ch13ex4muc
   :numbered: left
   :adaptive:
   :noindent:

   The following program segment should print the average value of a list. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   avg <- 0
   sum <- 0
   =====
   for each item in list
   =====
   sum <- item + sum
   =====
   if (length of list) >= 1
   =====
   avg <- sum / (length of list)
   =====
   DISPLAY(avg)
   =====
   avg <- sum / item #distractor


.. parsonsprob:: ch13ex5muc
   :numbered: left
   :adaptive:

   The following program segment should display who won the game based on the two players' scores. Arrange the code so that the first IF statement is for a Player 1 win, the second for a Player 2 win and the third for a tie.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   player1 <- 10
   player2 <- 10
   =====
   if player1 > player2
   =====
       DISPLAY("Player 1 wins!")
   =====
   if player1 < player2
   =====
       DISPLAY("Player 2 wins!")
   =====
   if player1 = player2
   =====
       DISPLAY("It's a tie!")


.. parsonsprob:: ch13ex6muc
   :numbered: left
   :adaptive:

   The following program segment should find and display the minimum value of a list. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   min <- list[0]
   =====
   for each item in list
   =====
       if item < min
   =====
       min <- item
   =====
   DISPLAY(min)
   =====
   if item > min #distractor
