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
	:prefix: 8-7-

Chapter 8 Exercises
--------------------

#. 

    .. tabbed:: ch8ex1t

        .. tab:: Question
            
            Fix the 5 syntax errors in the code below to print a countdown of the numbers from 10 to 0.  

            .. activecode:: ch8ex1q
                :nocodelens:

                counter = 10
                while Counter > 0:
                    Print(counter)
                    counter = Counter + 1                 

        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch8ex1q
                
#. 
   
    .. tabbed:: ch8ex2t

        .. tab:: Question

           Make 5 changes to the code below to correctly print a count up from -10 to 0.  
           
           .. activecode::  ch8ex2q
                :nocodelens:

                output = ""
                x = -10
                while x < 0
                    x = x - 1
                output = output + str(x) + " "
                print(output)
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex2q

#. 

    .. tabbed:: ch8ex3t

        .. tab:: Question

           Finish lines 1 and 5 so that the following code correct prints all the values from -5 to -1.  
        
           .. activecode::  ch8ex3q
                :nocodelens:
                
                output = 
                x = -5
                while x < 0:
                    output = output + str(x) + " "
                    x = 
                print(output)
                

        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch8ex3q
                
#. 

    .. tabbed:: ch8ex4t

        .. tab:: Question

           The code below is supposed to print an estimate of the square root.  But, the indention is wrong on 4 lines.  Fix it.
           
           .. activecode::  ch8ex4q
                :nocodelens:

                target = 6
                    guess = 2
                guessSquared = guess * guess
                while abs(target-guessSquared) > 0.01:
                    closer = target / guess
                guess = (guess + closer) / 2.0
                        guessSquared = guess * guess
                    print("Square root of", target,"is", guess)
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex4q
   
#. 

    .. tabbed:: ch8ex5t

        .. tab:: Question

           The program below is supposed to print the times tables for 1 to 3, but there are 5 errors.  Fix the errors.
           
           .. activecode::  ch8ex5q
                :nocodelens:

                for x in range(1,3):
                     for y in range(1,10)
                         print(str(x) + " * " str(y) + " = " x*y)


        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex5q
                
#. 

    .. tabbed:: ch8ex6t

        .. tab:: Question

           Rewrite the following code to use a while loop instead of a for loop.
           
           .. activecode::  ch8ex6q
                :nocodelens: 
                
                product = 1  # Start out with nothing
                numbers = range(1,11)
                for number in numbers:
                    product = product * number
                print(product)
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex6q
                
#. 

    .. tabbed:: ch8ex7t

        .. tab:: Question

           Rewrite the following code to use a while loop instead of a for loop. 
           
           .. activecode::  ch8ex7q
                :nocodelens: 
                
                # STEP 1: INITIALIZE ACCUMULATOR 
                product = 1  # init product to 1
                # STEP 2: GET DATA
                numbers = range(10,21,2)
                # STEP 3: LOOP THROUGH THE DATA
                for number in numbers:
    	            # STEP 4: ACCUMULATE
    	           product = product * number
                # STEP 5: PROCESS RESULT
                print(product) 
                    
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex7q
                
#. 

    .. tabbed:: ch8ex8t

        .. tab:: Question

           Modify the code below to create a function that will take numbers as input until you enter a negative number and then will return the average of the numbers.  
           
           .. activecode::  ch8ex8q
                :nocodelens:
                
                sum = 0
                count = 0
                message = "Enter an integer or a negative number to stop"
                value = input(message)
                while int(value) > 0:
                    print("You entered " + value)
                    sum = sum + int(value)
                    count = count + 1
                    value = input(message)
                print("The sum is: " + str(sum) + 
                      " the average is: " + str(sum / count))
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex8q
                
#. 

    .. tabbed:: ch8ex9t

        .. tab:: Question

           Create a function to calculate and return the sum of all of the even numbers from 1 to the passed input using a while loop.
           
           .. activecode::  ch8ex9q
                :nocodelens:
                                
        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex9q
                
#. 

    .. tabbed:: ch8ex10t

        .. tab:: Question

           Create a procedure to print stars in a square pattern and have it take as input the number of stars on a side.  Use a nested loop to do this.
           
           .. activecode::  ch8ex10q
               :nocodelens:

        .. tab:: Discussion 

            .. disqus::
                :shortname: studentcsp
                :identifier: studentcsp_ch8ex10q



