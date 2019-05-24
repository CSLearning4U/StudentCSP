.. qnum::
   :prefix: 25-4-
   :start: 1

Set #4
-------------------------------------

The following questions make up Set #4 of the Untimed Practice Exam Questions. The questions resemble, both in format and substance, what you might see on the AP CS Principles exam. You should finish these questions within 17 minutes to satisfy the time constraints of the AP exam. You may refer to the AP CS Reference Sheet, which can be found here_.

.. _here: raw::html <a href="" target="_blank">here</a>

Click the "Start" button when you are ready to begin the exam.  Click the "Pause" button to pause the exam (you will not be able to see the questions when the exam is paused).  It will show how much time you have used, but you have unlimited time.  Click on the "Finish Exam" button at the end when you are done.  The number correct, number wrong, and number skipped will be displayed at the bottom of the page.  Feedback for each answer will also be shown as well as your answer.

You will not be able to change your answers after you hit the "Finish Exam" button.


   .. mchoice:: e25_4_1
      :answer_a: Linear search is more efficient for large data sets than binary search.
      :answer_b: Binary search does not work on ordered sets.
      :answer_c: Linear search looks at one element at a time.
      :answer_d: Binary search is better for smaller sets.
      :correct: c
      :feedback_a: Incorrect. Linear search will generally take longer since it looks at one element at a time.
      :feedback_b: Incorrect. Binary search can be used on ordered sets.
      :feedback_c: Correct. Linear search looks at just one element at a time.
      :feedback_d: Incorrect. Linear search is generally preferred for smaller data sets.

      Which of the following is true about linear and binary search?



   .. mchoice:: e25_4_2
      :answer_a: An unsolvable problem cannot be solved using any algorithm.
      :answer_b: A solvable problem can be solved using an algorithm.
      :answer_c: Some solvable problems will not run in reasonable time.
      :answer_d: An unsolvable problem can be solved using an algorithm.
      :correct: b
      :feedback_a: Incorrect. If a problem is unsolvable, not even an algorithm can solve it.
      :feedback_b: Correct. An algorithm can solve an a solvable problem.
      :feedback_c: Incorrect. Some solvable problems will take long to solve with an algorithm and will, therefore, not run in reasonable time.
      :feedback_d: Incorrect. If a problem is unsolvable, an algorithm will not solve it.

      Which of the following statements is NOT true?



   .. mchoice:: e25_4_3
      :answer_a: Instructions may involve variables which may change or be output from the program.
      :answer_b: Instructions are processed sequentially.
      :answer_c: A program always has a return value.
      :answer_d: A program automates processes in a computer.
      :correct: c
      :feedback_a: Incorrect. A program can have variables which may be changed or be output by the program.
      :feedback_b: Incorrect. Code in a program is read sequentially line by line.
      :feedback_c: Correct. A return value is not a necessity for a program.
      :feedback_d: Incorrect. A program is an automated process that runs on a computer.

      Which of the following is NOT true about a program?


   .. mchoice:: e25_4_4
      :answer_a: In no situation; this procedure works as intended
      :answer_b: In all situations; this procedure will DISPLAY the maximum, not the minimum
      :answer_c: If every item in the list is positive
      :answer_d: If every item in the list is negative
      :correct: c
      :feedback_a: Incorrect. This procedure does not work in every case.
      :feedback_b: Incorrect. This code does obtain a minimum value, but fails to do so under certain circumstances.
      :feedback_c: Correct. If every item in the list is positive, "min" never gets updated because it is initialized to 0 and every value in the list is being compared to it.
      :feedback_d: Incorrect. The code will work as intended if every value is negative.

      Imagine you want to create a procedure to find and print the smallest item in a list. Take the code below for example:


      ::

	       PROCEDURE showMin(aList)

	        {
	         min ← 0

	         FOR EACH item IN aList

	          {
	           if (min > item)

	            {
		            min ← item
	            }
	          }
	         DISPLAY(“smallest item in list is “ + min)
	        }

      In what situation would this procedure fail to correctly display the minimum?



   .. mchoice:: e25_4_5
      :answer_a: Abstraction reduces or removes details to help understand something new.
      :answer_b: A lower-level abstraction is less specific.
      :answer_c: Abstraction helps you manage the details and code of a program.
      :answer_d: Lower-level abstractions can be combined to make higher-level abstractions.
      :correct: b
      :feedback_a: Incorrect. Abstraction removes unnecessary information that is not needed to understand something.
      :feedback_b: Correct. The lower the level, the more detail.
      :feedback_c: Incorrect. Abstraction is a way of managing details because it emphasizes the details that are relevant.
      :feedback_d: Incorrect. Since lower-level abstractions are more detailed, they cannot be combined to make higher-level abstractions.

      Which of the following is NOT true about abstraction?


   .. mchoice:: e25_4_6
      :answer_a: All digital data is an abstraction.
      :answer_b: All data eventually becomes binary digits (bits) that the computer interprets.
      :answer_c: Programming commands are a potential source of bits.
      :answer_d: Abstractions occur only in hardware applications.
      :correct: d
      :feedback_a: Incorrect. Digital data is represented by abstractions at different levels.
      :feedback_b: Incorrect. Computers read binary digits to interpret data.
      :feedback_c: Incorrect. Commands are data which can be broken down into bits.
      :feedback_d: Correct. Abstractions occur in software applications.

      Which of the following is NOT true?

   .. mchoice:: e25_4_7
      :answer_a: Binary (base 2)
      :answer_b: Tertiary (base 3)
      :answer_c: Hexadecimal (base 16)
      :answer_d: Decimal (our number system)
      :correct: b
      :feedback_a: Incorrect. The binary number system is commonly used in computer programming.
      :feedback_b: Correct. The tertiary (base 3) number system is not used in computer programming.
      :feedback_c: Incorrect. The hexadecimal number system is used because it is easy to convert into the binary and decimal systems.
      :feedback_d: Incorrect. The decimal system is used in computer programs.


      Which of the following number systems is NOT used in a computer program?




   .. mchoice:: e25_4_8
      :answer_a: Converting data usually comes at a cost.
      :answer_b: Data is never lost in conversion.
      :answer_c: Data is never changed in conversion.
      :answer_d: Data can always be converted without a loss.
      :correct: a
      :feedback_a: Correct. When converting, things such as the quality of the data may be compromised.
      :feedback_b: Incorrect. Data can be lost when converting across types.
      :feedback_c: Incorrect. Data may lose readability in conversion and may be changed as a result.
      :feedback_d: Incorrect. There are instances in which data is lost through conversion.

      Which of the following is true?



   .. mchoice:: e25_4_9
      :answer_a:
      :answer_b:
      :answer_c:
      :answer_d:
      :correct: a
      :feedback_a: Correct. This is a repeating decimal which will result in an overflow error.
      :feedback_b: Incorrect. Though the solution is undefined, it will not result in an overflow error.
      :feedback_c: Incorrect. This will not result in an overflow error but rather a value error.
      :feedback_d: Incorrect. This will result in an infinite loop.

      Which of the following is most likely an example of an overflow error?

      ::


        (A)

        z ← ⅓


        (B)

        z ← 1/0


        (C)

        nums ← (1, 2, 3)

        n ← 0

        REPEAT 4 TIMES

        n ← n + 1

        DISPLAY(nums(n))


        (D)

        n ← 0

        REPEAT UNTIL NOT n = 0

        n ← n * 100




   .. mchoice:: e25_4_10
      :answer_a: Problems that have a “yes” or “no” answer for all inputs are called decidable.
      :answer_b: Problems that have a “yes” or “no” answer for all inputs are called undecidable.
      :answer_c: Undecidable problems always have a solution.
      :answer_d: Problems that cannot be solved with an algorithm are called solvable.
      :correct: a
      :feedback_a: Correct. A decidable problem is solvable in finite steps.
      :feedback_b: Incorrect. If a problem is solvable, it cannot be undecidable.
      :feedback_c: Incorrect. It is impossible to construct an algorithm that solves an undecidable problem.
      :feedback_d: Incorrect. Problems than cannot be solved with an algorithm are called unsolvable.

      Which of the following statements is true?


   .. mchoice:: e25_4_11
      :answer_a: 11100101
      :answer_b: 10100111
      :answer_c: 0000111
      :answer_d: 1010101
      :correct: b
      :feedback_a: Incorrect. 11100101 = (1 × 2⁷) + (1 × 2⁶) + (1 × 2⁵) + (0 × 2⁴) + (0 × 2³) + (1 × 2²) + (0 × 2¹) + (1 × 2⁰) = 229
      :feedback_b: Correct. 10100111 = (1 × 2⁷) + (0 × 2⁶) + (1 × 2⁵) + (0 × 2⁴) + (0 × 2³) + (1 × 2²) + (1 × 2¹) + (1 × 2⁰) = 167
      :feedback_c: Incorrect. 0000111 = (0 × 2⁶) + (0 × 2⁵) + (0 × 2⁴) + (0 × 2³) + (1 × 2²) + (1 × 2¹) + (1 × 2⁰) = 7
      :feedback_d: Incorrect. 1010101 = (1 × 2⁶) + (0 × 2⁵) + (1 × 2⁴) + (0 × 2³) + (1 × 2²) + (0 × 2¹) + (1 × 2⁰) = 85

      Which of the following correctly converts 167 to the binary number system? (Hint: Binary numbers have place values that are powers of 2.)


   .. mchoice:: e25_4_12
      :answer_a: Expected to run in reasonable time
      :answer_b: NOT expected to run in reasonable time
      :answer_c: Impossible to calculate
      :answer_d: Easier to do by hand
      :correct: b
      :feedback_a: Incorrect. Algorithms with exponential will continually change with respect to time.
      :feedback_b: Correct. Since exponential behavior implies continual change, it may not run in reasonable time.
      :feedback_c: Incorrect. They can be solved for a specific time.
      :feedback_d: Incorrect. It is not necessarily easier to calculate by hand.

      Algorithms will exponential behavior (e.g. x^n) are:


   .. mchoice:: e25_4_13
      :answer_a: Lossy
      :answer_b: Lossless
      :answer_c: Data manipulation
      :answer_d: Sticky
      :correct: b
      :feedback_a: Incorrect. Data is lost in lossy compression.
      :feedback_b: Correct. All original data can be retrieved through lossless compression.
      :feedback_c: Incorrect. Data manipulation is not a specific form of data compression.
      :feedback_d: Incorrect. There is no such thing as sticky data compression.

      Data compression that allows for all of the original data to be retrieved is called:



   .. mchoice:: e25_4_14
      :answer_a: The internet
      :answer_b: A network
      :answer_c: A model
      :answer_d: Memory
      :correct: b
      :feedback_a: Incorrect. The internet is the global system of connected computer networks.
      :feedback_b: Correct. A network is a grouping of multiple systems.
      :feedback_c: Incorrect. A model represents entities and the relationships between them.
      :feedback_d: Incorrect. Memory is the storing of information.


      A group of two or more systems linked together is called:


   .. mchoice:: e25_4_15
      :answer_a: 0
      :answer_b: 22
      :answer_c: 16
      :answer_d: 4
      :correct: c
      :feedback_a: Incorrect. The block of code will repeat 3 times and the value of n will be 16.
      :feedback_b: Incorrect. The block of code will repeat 3 times and the value of n will be 16.
      :feedback_c: Correct. The block of code will repeat 3 times and the value of n will be 16.
      :feedback_d: Incorrect. The block of code will repeat 3 times and the value of n will be 16.

      What is the value of n after the above code executes?

      ::


        i ← 1

        n ← 2

        REPEAT until i = 4

          {
          n ← n * 2

          i ← i + 1
          }
