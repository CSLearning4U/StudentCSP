..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".

.. 	qnum::
	:start: 1
	:prefix: csp-8-5-
	
.. highlight:: java
   :linenothreshold: 4

	   	  
Nested For Loops
=================

The body of any loop, can even include...another loop!  Here is a super-simple program that generates all the times tables from 0 to 10.  The ``str()`` function changes a numeric value into a string.

.. codelens:: Times_Table
	:showoutput: 

	for x in range(0,11):
	    for y in range(0,11):
	        print(str(x) + " * " + str(y) + " = " + str(x*y))
		

Here are two different ways to look at this program.  In the first one, we look at the *structure* of the program -- what you can understand by just *looking* at the program.

.. the video is nestedLoopStructure.mov

.. youtube:: IKh1TdYL3o0
    :width: 640
    :height: 480
    :align: center

In this video, we look at the *execution* of the program -- how it actually works when it's being *run* by the computer.

.. the video is nestedLoopTrace.mov

.. youtube:: mIolNVIF1A4
    :width: 640
    :height: 480
    :align: center
	   
How Many Times Does the Inner Loop Execute?
--------------------------------------------
		   
Try out the following code.  How many ``*``'s are printed?  Why do you think it prints that many?  Try changing the start and end values and see what changing those does to the output.

.. activecode:: Nested_Loops_Stars

    for x in range(0,2):
        for y in range(0,3):
            print('*')
            

The outer loop executes 2 times and each time the outer loop executes the inner loop executes 3 times so this will print 2 * 3 = 6 stars.  

.. note::
   The formula for calculating the number of times the inner loop executes is the number of times the outer loop repeats multiplied by the number of times the inner loop repeats.
		   
.. mchoice:: 8_5_1_NumStars
   :practice: T
   :answer_a: 6
   :answer_b: 9
   :answer_c: 12
   :answer_d: 16
   :answer_e: 20
   :correct: c
   :feedback_a: Remember that the range function will include the start value and all the numbers up to one less than the end value.  So the outer loop will execute 3 times ([0,1,2]).
   :feedback_b: This would be true if they were both range(0,3).  Is that correct?
   :feedback_c: The number of times a nested loop executes is the number of times the outer loop executes (3) times the number of the times the inner loop executes (4) so that is 3 * 4 = 12.  
   :feedback_d: This would be true if both were range(0,4).  Is that right?
   :feedback_e: This would be true if the range returned all the numbers from start to end, but it does not.

   How many times will this loop print a ``*``?
   
   :: 
      
       for x in range(0,3):
           for y in range(0,4):
               print('*')
               
You can add items to a string in the inner loop and then print the strings to make a pattern.  
               
.. activecode:: Nested_Loops_Pattern

    for x in range(0,2):
        line = ""
        for y in range(0,3):
            line = line + '*'
        print(line)
        
Modify the code above to draw a square of stars.  

.. tabbed:: 8_5_2_WSt

        .. tab:: Question

           Write code to print stars in the shape of an empty square of size 4 by 4. 
           
           .. activecode::  8_5_2_WSq
                :nocodelens:

        .. tab:: Answer
            
          .. activecode::  8_5_2_WSa
              :nocodelens:
              
              # TOP LINE 
              line = ""
              for x in range(0,4):
                line = line + "*"
              print(line)

              # MIDDLE LINES 
              for x in range(0,2):      # outer loop for edge of square 
                line = "*"
                for y in range(0,2):    # inner loop for space in square
                    line = line + ' '
                line = line + '*'
                print(line)

              # BOTTOM LINE 
              line = ""
              for x in range(0,4):
                line = line + "*"
              print(line)

                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_8_5_2_WSq
               
.. note::

    Discuss topics in this section with classmates. 

      .. disqus::
          :shortname: cslearn4u
          :identifier: studentcsp_8_5