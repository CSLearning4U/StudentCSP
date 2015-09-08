..  Copyright (C)  Brad Miller, David Ranum, Jeffrey Elkner, Peter Wentworth, Allen B. Downey, Chris
    Meyers, and Dario Mitchell.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".
    

.. setup for automatic question numbering.

.. 	qnum::
	:start: 1
	:prefix: 10-6-

Chapter 10 Exercises
---------------------

#. 

    .. tabbed:: ch10ex1t

        .. tab:: Question
            
            Fix 4 syntax errors in the code below to correctly draw a square

            .. activecode:: ch10ex1q
                :nocodelens:

                from turtle import 	    # use the turtle library
                space = screen()   		# create a turtle space
                alisha = Turtle  		# create a turtle named alisha
                alisha.setheading(90)  	# point due north
                for sides in [1,2,3]:	# repeat the indented lines 4 times
    	            alisha.forward(100)        	# move forward by 100 units
      	            alisha.right(90)           	# turn by 90 degrees
      	            
        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch10ex1q
                
#. 
   
    .. tabbed:: ch10ex2t

        .. tab:: Question

           Fix the code below to draw a rectangle. You will need to fix the indention on 3 lines. 
           
           .. activecode::  ch10ex2q
                :nocodelens:

                from turtle import *       
                    space = Screen()
                carlos = Turtle()
                
                # repeat 2 times
                for i in [1,2]:  
                    carlos.forward(175)
                    carlos.right(90)
                carlos.forward(150)
                carlos.right(90)

                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex2q

#. 

    .. tabbed:: ch10ex3t

        .. tab:: Question

           Fill in values for ``x`` on line 5 and ``y`` on line 7 to allow the code below to correctly draw a pentagon.     
        
           .. activecode::  ch10ex3q
                :nocodelens:
                
                from turtle import *   	# use the turtle library
                space = Screen()    	# create a turtle space
                will = Turtle()   		# create a turtle named will
                will.setheading(90)    	# point due north
                for sides in range(x):	# repeat the indented lines 
      	            will.forward(100)      	# move forward by 100 units
      	            will.right(y)          
         

        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch10ex3q
                
#. 

    .. tabbed:: ch10ex4t

        .. tab:: Question

           Finish the code on lines 1, 2, 3, 6 and 8 below to correctly draw a triangle.  
           
           .. activecode::  ch10ex4q
                :nocodelens:

                from        
                space =
                marie = 
  
                # repeat
                for i in range(): 
                    marie.forward(100)
                    marie.left()
          
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex4q
   
#. 

    .. tabbed:: ch10ex5t

        .. tab:: Question

           Fix the indention in the code below to correctly draw 20 pentagons.  
           
           .. activecode::  ch10ex5q
                :nocodelens:

                from turtle import *     # use the turtle library
                from sys import *        # use the system library
                setExecutionLimit(50000) # let this take up to 50 seconds
                space = Screen()         # create a turtle space
                zoe = Turtle()           # create a turtle named zoe
                zoe.setheading(90)       # point due north
    
                for repeats in range(20):   # draw the pattern 20 times
      	            zoe.forward(10)         	# Offset the shapes a bit
      	            zoe.right(18)             	# And turn each one a bit
      
      	        # This part makes a pentagon
      	        for sides in range(5):    # repeat 5 times
      	            zoe.forward(50)         # move forward by 50 unit
      	            zoe.right(72)           # turn by 72 degrees

        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex5q
                
#. 

    .. tabbed:: ch10ex6t

        .. tab:: Question

           Fix the following code below to draw a circle of turtles using the ``stamp`` procedure.  You will need to change 3 lines. 
           
           .. activecode::  ch10ex6q
                :nocodelens: 
                
                from turtle import *
                space = Screen()
                jose = Turtle()
                jose.shape("turtle")
                jose.               
                for size in range():   
                    jose.forward(50)
                    jose.stamp()        
                    jose.forward()
                    jose.right(36)
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex6q
                
#. 

    .. tabbed:: ch10ex7t

        .. tab:: Question

           Rewrite the following code to create a procedure to draw a square with a turtle.  Pass the turtle and the size of the square as input (parameters) to the procedure. 
           
           .. activecode::  ch10ex7q
                :nocodelens: 
                
                from turtle import *	# use the turtle library
                space = Screen()   		# create a turtle space
                alisha = Turtle()  		# create a turtle named alisha
                alisha.setheading(90)  	# point due north
                for sides in [1,2,3,4]:	# repeat the indented lines 4 times
    	            alisha.forward(100)        	# move forward by 100 units
      	            alisha.right(90)           	# turn by 90 degrees
                        
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex7q
                
#. 

    .. tabbed:: ch10ex8t

        .. tab:: Question

           Rewrite the following code to create a procedure to draw a rectangle with a turtle.  Pass the turtle and the length and width of the rectangle as parameters to the procedure. 
           
           .. activecode::  ch10ex8q
                :nocodelens:
                
                from turtle import *       
                space = Screen()
                carlos = Turtle()
                
                # repeat 2 times
                for i in [1,2]:  
                    carlos.forward(175)
                    carlos.right(90)
                    carlos.forward(150)
                    carlos.right(90)
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex8q
                
#. 

    .. tabbed:: ch10ex9t

        .. tab:: Question

           Create a procedure to draw 4 turtles at the 4 corners of a square using the ``stamp`` procedure.  
           
           .. activecode::  ch10ex9q
                :nocodelens:
                                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex9q
                
#. 

    .. tabbed:: ch10ex10t

        .. tab:: Question

           Write a procedure that takes a turtle and a number of sides as parameters and draws a polygon with that number of sides. 
           
           .. activecode::  ch10ex10q
               :nocodelens:
                                 
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch10ex10q



