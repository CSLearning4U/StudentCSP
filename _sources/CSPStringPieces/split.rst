..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".
    
.. 	qnum::
	:start: 1
	:prefix: csp-17-3-

Using the Split Function
===================================

The ``split`` function does exactly that.  It takes as input the character to split on, then returns a *list* with pieces.  The pieces can then be *indexed*.

Try running this program.

.. activecode:: firstsplit
   :tour_1: "Line by line tour"; 2: StP1-line1; 5: StP1-line2; 8: StP1-line3; 9: StP1-line4; 10: StP1-line5;

   # create the input
   input = "Pat,Smith,girl,65 Elm Street,eat"
   
   # split on the comma
   pieces = input.split(",")
   
   # print the values
   print(pieces)
   print("First name is:")
   print(pieces[0])

.. mchoice:: 17_3_1_question_firstsplit
   :practice: T
   :answer_a: Smith
   :answer_b: girl
   :answer_c: 65 Elm Street
   :answer_d: eat
   :answer_e: We would get an error
   :correct: c
   :feedback_a: That's pieces[1].
   :feedback_b: That's pieces[2]
   :feedback_c: The address is at position 3 in the resulting list.
   :feedback_d: That's pieces[4]
   :feedback_e: Why would this cause an error?  We can use indices to get the element at an index in a list.

   What do you think we would get if we executed ``print(pieces[3])``

.. mchoice:: 17_3_2_question_firstsplit2
   :practice: T
   :answer_a: Smith
   :answer_b: girl
   :answer_c: 65 Elm Street
   :answer_d: eat
   :answer_e: We would get an error
   :correct: e
   :feedback_a: That's pieces[1].
   :feedback_b: That's pieces[2].
   :feedback_c: That's pieces[3].
   :feedback_d: That's pieces[4].
   :feedback_e: The error happens because that index is past the end of the list.  The last item is at index 4.

   What do you think we would get if we executed ``print(pieces[5])``
   
The code below is the first activecode modified to use the ``split`` function to assign the values to the variables.

.. activecode:: madlib1_split
   :tour_1: "Structural tour"; 2: StP1-line1; 5: StP1-line2; 8-12: StP2-line3-7; 15-19: StP2-line8-12; 22-26: StP2-line13-17;

   # create the input
   input = "Pat,Smith,girl,65 Elm Street,eat"
   
   # split at the comma
   pieces = input.split(",")
   
   # initialize the variables
   firstName = pieces[0]
   lastName = pieces[1]
   gender = pieces[2]
   address = pieces[3]
   verb = pieces[4]
   
   # create the story
   start = "Once there was a " + gender + " named " + firstName + "."
   next1 = "A good " + gender + " living at " + address + "."
   next2 = "One day, a wicked witch came to the " + lastName + " house."
   next3 = "The wicked witch was planning to " + verb + " " + firstName + "!"
   ending = "But " + firstName + " was smart and avoided the wicked witch."
   
   # print the story
   print(start)
   print(next1)
   print(next2)
   print(next3)
   print(ending)

This makes it easy to change all of the data, by changing only one line as shown below.

.. activecode:: madlib1_split2
   :tour_1: "Structural tour"; 2: StP3-line1; 5: StP1-line2; 8-12: StP2-line3-7; 15-19: StP2-line8-12; 22-26: StP2-line13-17;

   # create the input
   input = "Abe,Brown,boy,1313 Maple Lane,trick"
   
   # split at the comma
   pieces = input.split(",")
   
   # initialize the variables
   firstName = pieces[0]
   lastName = pieces[1]
   gender = pieces[2]
   address = pieces[3]
   verb = pieces[4]
   
   # create the story
   start = "Once there was a " + gender + " named " + firstName + "."
   next1 = "A good " + gender + " living at " + address + "."
   next2 = "One day, a wicked witch came to the " + lastName + " house."
   next3 = "The wicked witch was planning to " + verb + " " + firstName + "!"
   ending = "But " + firstName + " was smart and avoided the wicked witch."
   
   # print the story
   print(start)
   print(next1)
   print(next2)
   print(next3)
   print(ending)

.. tabbed:: 17_3_3_WSt

        .. tab:: Question

           Write code to print out the phone number without the area code using the ''split'' function. 
           
           .. activecode::  17_3_3_WSq
               :nocodelens:

        .. tab:: Answer
            
          .. activecode:: 17_3_3_WSa
              :nocodelens:
                
              # create the input
              input = "(805)555-8585"

              # split on the close-parenthesis
              phoneNumber = input.split(")")

              # print the value
              print("My number is:")
              print(phoneNumber[1])
                                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_17_3_3_WSq

.. note::

    Discuss topics in this section with classmates. 

      .. disqus::
          :shortname: cslearn4u
          :identifier: studentcsp_17_3

   

