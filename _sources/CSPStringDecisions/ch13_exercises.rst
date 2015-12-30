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
	:prefix: 13-6-

Chapter 13 Exercises
---------------------

#. 

    .. tabbed:: ch13ex1t

        .. tab:: Question
            
            Fix 7 problems in the code below so that it runs.   

            .. activecode:: ch13ex1q
                :nocodelens:

                score = 20
                if score < 10
                print("You can do better.")
                if score > 10:
                print(Good job!")
                if score > 20
                print("Amazing"
      	            
    

        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex1q

#. 

    .. tabbed:: ch13ex2t

        .. tab:: Question

           Fix 6 errors in the code below so that it works correctly.  
           
           .. activecode::  ch13ex2q
                :nocodelens:

                print(You are in front of a creepy door in a hallway.")
                prin("What do you want to do?")
                action = input ("Type: in, left, or right. Then click OK or press enter)
                if action == "in"
                    print("You choose to go in.")
                    print("The room is pitch black.")
                if action == "left":
                print("You choose to turn left.")
                    print("A ghost appears at the end of the hall.")
                if action == "right":
                    print("You choose to turn right.")
                print("A greenish light is visible in the distance.")
          
      
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex2q

#. 

    .. tabbed:: ch13ex3t

        .. tab:: Question

           Fix the code below to assign grades correctly using elif and else. 
        
           .. activecode::  ch13ex3q
                :nocodelens:
                
                score = 80
                if score >= 90:
                    grade = "A"
                if score >= 80:
                    grade = "B"
                if score >= 70:
                    grade = "C"
                if score >= 60:
                    grade = "D"
                if score < 60:
                   grade = "E"
                print(grade)
                         
         

       



        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex3q
                
#. 
                
    .. tabbed:: ch13ex4t

        .. tab:: Question

           Change the code below to use elif and else rather than several ifs.  Also fix it to print "Good job!" if the score is greater than 10 and less than or equal to 20 and "Amazing" if the score is over 20.   
           
           .. activecode::  ch13ex4q
                :nocodelens:

                score = 22
                if score < 10:
                    print("You can do better.")
                if score > 10:
                    print("Good job!")
                if score > 20:
                    print("Amazing")


       
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex4q
                

   
#. 

    .. tabbed:: ch13ex5t

        .. tab:: Question

           Change the code below to use ``elif`` and ``else``.  
           
           .. activecode::  ch13ex5q
                :nocodelens:

                num = input ("Type a number from 1 to 5. Then click OK or press enter")
                if num == "1":
                    print("You will get a treat.")
                if num == "2":
                    print("You will lose something.")
                if num == "3":
                    print("You will meet a new friend.")
                if num == "4":
                    print("You will catch a cold.")
                if num == "5":
                    print("You will ace a test.")

       

        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex5q
                
#. 

    .. tabbed:: ch13ex6t

        .. tab:: Question

           Change the following code to use ``elif`` and ``else`` instead.  
           
           .. activecode::  ch13ex6q
                :nocodelens: 
                
                team1 = 20
                team2 = 20
                if (team1 < team2):
                    print("team1 won")
                if (team2 > team1):
                    print("team2 won")
                if (team2 == team1):
                    print("team1 and team2 tied")

    
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex6q
                
#. 

    .. tabbed:: ch13ex7t

        .. tab:: Question

           Change the code below to use ``elif`` and ``else``.  
           
           .. activecode::  ch13ex7q
                :nocodelens: 
                
                x = .25
                if x <= .25:
                    print("x is in the first quartile - x <= .25")
                if x <= .5 and x > .25:
                    print("x is in the second quartile - .25 < x <= .5")
                if x <= .75 and x > .5:
                    print("x is in the third quartile - .5 < x <= .75")
                if x > .75:
                    print("x is in the fourth quartile - .75 < x <= 1")
                
                

    
                
                
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex7q
                
#. 

    .. tabbed:: ch13ex8t

        .. tab:: Question

           Change the code below into a procedure that takes a number as a parameter and prints the quartile.  Be sure to test each quartile.
           
           .. activecode::  ch13ex8q
                :nocodelens:
                
                x = .25
                if x <= .25:
                    print("x is in the first quartile - x <= .25")
                if x <= .5 and x > .25:
                    print("x is in the second quartile - .25 < x <= .5")
                if x <= .75 and x > .5:
                    print("x is in the third quartile - .5 < x <= .75")
                if x > .75:
                    print("x is in the fourth quartile - .75 < x <= 1")

       
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex8q
                
#. 

    .. tabbed:: ch13ex9t

        .. tab:: Question

           Write a function that will take a number as input and return a fortune as a string.  Ask the user to pick a number to get the fortune before you call the function.  Have at least 5 different fortunes.  Use ``if``, ``elif``, and ``else``.  
           
           .. activecode::  ch13ex9q
                :nocodelens:

        
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex9q
                
#. 

    .. tabbed:: ch13ex10t

        .. tab:: Question

           Write a procedure to tell an interactive story and let the user choose one of at least 3 options.  
           
           .. activecode::  ch13ex10q
               :nocodelens:

       
                                 
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch13ex10q



