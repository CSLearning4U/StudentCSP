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
	:prefix: 16-11-

Chapter 16 Exercises
---------------------

#. 

    .. tabbed:: ch16ex1t

        .. tab:: Question
            
            Fix syntax 6 errors in the code below so that the code runs correctly. It should set ``combined`` to the concatenation of ``start`` and ``name``.  It should print the length of the combined string, print the combined string, and it should print the result of ``name * 3``. 

            .. activecode:: ch16ex1q
                :nocodelens:
                
                name = 'Mark"
                start = "My name is '
                combined = start  name
                print(len(combined)
                print(combined)
                print name * 3
      	            
                
        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex1q

#. 

    .. tabbed:: ch16ex2t

        .. tab:: Question

           Fix the 5 syntax errors in the code below so that it runs.  It should print the length of ``myFirstList`` and print the result of ``myFirstList * 3``.  Then it should set ``mySecondList`` to the concatenation of ``myFirstList`` and a list containing ``321.4``.  Then it should print the value of ``mySecondList``.
           
           .. activecode::  ch16ex2q
                :nocodelens:

                myFirstList = [12,"ape"13]
                print(len(myFirstList)
                print(myfirstList * 3)
                mySecondList = myFirstList + [321.4
                print(mySecondList
                
          
       
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex2q
                
#. 

    .. tabbed:: ch16ex3t

        .. tab:: Question

           Fix 5 syntax errors in the code below so that it runs and prints the contents of ``items``.  
           
           .. activecode::  ch16ex3q
                :nocodelens:

               items = [2,4,6 8]
               items[0] = "First item'
               items[1] = items0]
               items[2] = items[2] + 1
               print items 

       
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex5q

#. 

    .. tabbed:: ch16ex4t

        .. tab:: Question

           Fix the indention in the code below so that it runs correctly.  It should loop and add the current value of ``source`` to ``soFar`` each time through the loop.  It should also print the value of ``soFar`` each time through the loop.
        
           .. activecode::  ch16ex4q
                :nocodelens:
                
                source = ["This","is","a","list"]
                soFar = []
                for index in range(0,len(source)):
                soFar = [source[index]] + soFar
                print(soFar)

     

        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex3q
                
#. 
                
    .. tabbed:: ch16ex5t

        .. tab:: Question

           Fix 4 syntax errors in the code below.  After the code executes the list ``soFar`` should contain the reverse of the ``source`` list.  
           
           .. activecode::  ch16ex5q
                :nocodelens:

                # setup the source list
                source = ["This","is" "a","list"]
  
                # Set the accumulator to the empty list
                soFar = [
  
                # Loop through all the items in the source list
                for index in range(0,len(source))
  
                    # Add the current item in the source and print the current items in soFar
                    soFar = [source[index]] + sofar
                    print(soFar)


    
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex4q
                
                
#. 

    .. tabbed:: ch16ex6t

        .. tab:: Question

           Change the following code into a function.  It should take the list and return a list of the values at the even indicies.
           
           .. activecode::  ch16ex6q
                :nocodelens: 
                
                numbers = [0,1,2,3,4,5,6,7,8,9,10]
                evenList = []
                for index in range(0,len(numbers),2):
                    evenList = evenList + [numbers[index]]
                print(evenList)
                 
                
     

       
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex6q
                
#. 

    .. tabbed:: ch16ex7t

        .. tab:: Question

           Change the following into a procedure. It prints a countdown from 5 to 0.  Have it take the starting number for the countdown as a parameter.  Print each value till it gets to 0.
           
           .. activecode::  ch16ex7q
                :nocodelens: 
                
                for index in range(5, -1, -1):
                    print(index)


                

       
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex7q
                
#. 

    .. tabbed:: ch16ex8t

        .. tab:: Question

           Write a function that returns the values at the odd indices in a list.  The function should take the number list as a parameter.  If it is passed [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] for example, it should return [1, 3, 5, 7, 9].  
           
           .. activecode::  ch16ex8q
                :nocodelens:
                
                
       
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex8q
                
#. 

    .. tabbed:: ch16ex9t

        .. tab:: Question

           Write a function that takes a list of numbers and returns the sum of the positive numbers in the list.
            
           .. activecode::  ch16ex9q
                :nocodelens:

       
                            
                                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex9q
                
#. 

    .. tabbed:: ch16ex10t

        .. tab:: Question

           Write a function to return the reverse of a list, but with only every other item from the original list starting at the end of the list.  So, if it is passed the list [0,1,2,3,4,5] for example, it should return the list [5, 3, 1]. 
           
           .. activecode::  ch16ex10q
               :nocodelens:

       
         
                                 
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch16ex10q



