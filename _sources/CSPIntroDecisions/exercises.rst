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
	:prefix: 12-10-

Chapter 12 Exercises
---------------------

#.

    .. tabbed:: ch12ex1t

        .. tab:: Question

            Fix 3 syntax errors in the code below so that it correctly prints "x is less than 3" and then "All done" when x is less than 3.

            .. activecode:: ch12ex1q
                :nocodelens:

                x = 0
                if x < 3
                print ("x is less than 3")
                print ("All done)

        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: teachercsp_ch12ex1q

#.

    .. tabbed:: ch12ex2t

        .. tab:: Question

            The code currently prints "Hello" when the number is less than 3. Change it so that it prints "Hello" when the number is equal to 3.

            .. activecode::  ch12ex2q
                :nocodelens:

                x = 3
                if x < 3:
                    print("Hello")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex2q

#.

    .. tabbed:: ch12ex3t

        .. tab:: Question

           Fix the indention in the code below to use a price of 1.45 if the weight is less than 1 and a price of 1.15 otherwise.  There is also one syntax error.

           .. activecode::  ch12ex3q
                :nocodelens:

                weight = 0.5
                if weight < 1:
                price = 1.45
                if weight >= 1
                price = 1.15
                total = weight * price
                print(weight)
                print(price)
                print(total)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex3q

#.

    .. tabbed:: ch12ex4t

        .. tab:: Question

            Fill in line 1 with a weight that will make the total equal 1, and fix the indentation errors.

            .. activecode::  ch12ex4q
                :nocodelens:

                weight =

                if weight >= .5:
                price = 2
                if weight < .5:
                price = 1
                    total = weight * price
                    print(total)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex4q

#.

    .. tabbed:: ch12ex5t

        .. tab:: Question

           Fix 3 errors with indention in the code below to correctly set the price to 1.5 if the weight is less than 2 and otherwise set it to 1.3.

           .. activecode::  ch12ex5q
                :nocodelens:

                weight = 0.5
                numItems = 5
                if weight < 2:
                price = 1.50
                if weight >= 2:
                price = 1.30
                total = weight * price
                print(weight)
                    print(price)
                print(total)

        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: teachercsp_ch12ex5q

#.

    .. tabbed:: ch12ex6t

        .. tab:: Question

            The code currently does not do anything if the number is equal to 2. Fix it so that it prints "Hey" if the number is 2.

            .. activecode::  ch12ex6q
                :nocodelens:

                x = 2
                if x < 2:
                    print("Hello")
                if x > 2:
                    print("Hey")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex6q

#.

    .. tabbed:: ch12ex7t

        .. tab:: Question

           Fix 4 errors in the code below to print "x is a number from 	1 to 10" when x is greater than or equal to 1 and less than or equal to 10.

           .. activecode::  ch12ex7q
                :nocodelens:

                x = 3
                if x > 1 and x <= 10
                print ("x is a number from 1 to 10")
                    print ("All done")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex7q

#.

    .. tabbed:: ch12ex8t

        .. tab:: Question

            The following code prints "This is not 8" when the number is not 8. Change the if statement, so that it does the same thing but only uses one expression (No "and" or "or").

            .. activecode::  ch12ex8q
                :nocodelens:

                x = 8
                if x < 8 or x > 8:
                    print("This is not 8")
                else:
                    print("This is 8")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex8q

#.

    .. tabbed:: ch12ex9t

        .. tab:: Question

           Finish the conditional on line 3 to print "You can go out!" if either cleanedRoom or finishedHomework is true (not 0). It should always print "All done" as well.

           .. activecode::  ch12ex9q
                :nocodelens:

                cleanedRoom = 1
                finishedHomework = 0
                if
                    print ("You can go out!")
                print ("All done")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex9q

#.

    .. tabbed:: ch12ex10t

        .. tab:: Question

            Complete the conditional and fix the errors so that it prints "Good job" when the number is between 1 and 10 (inclusive) or is 15 and "Fail" when it is not.

            .. activecode::  ch12ex10q
                :nocodelens:

                x = 8
                    if
                print("Good job")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex10q

#.

    .. tabbed:: ch12ex11t

        .. tab:: Question

           Fix 5 errors in the following code to set the price to 1.45 if the weight is less than or equal to 1 and otherwise set it to 1.15.

           .. activecode::  ch12ex11q
                :nocodelens:

                weight = 0.5
                if weight < 1:
                price = 1.45
                if weight > 1:
                price = 1.15
                total = weight * price
                print(weigh)
                print(Price)
                print(total)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex11q

#.

    .. tabbed:: ch12ex12t

        .. tab:: Question

            Fix the indentation below, so that the code sets the price based off the weight, then checks if the total is greater than the amount in your wallet.

            .. activecode::  ch12ex12q
                :nocodelens:

                weight = 0.5
                numItems = 5
                wallet = 2

                if weight < 1:
                    price = 1.45
                    if weight >= 1:
                    price = 1.15
                    total = numItems * price
                    if total > wallet:
                    print("You have no money")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex12q

#.

    .. tabbed:: ch12ex13t

        .. tab:: Question

           Change 3 lines in the code below to correctly set the grade so that a 90 and above is an A, 80-89 is a B, 70 - 79 is a C, 60-69 is a D and below 60 is an E.

           .. activecode::  ch12ex13q
                :nocodelens:

                score = 93
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
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex13q

#.

    .. tabbed:: ch12ex14t

        .. tab:: Question

            Fix the errors in the code, and change it, so there's only 1 if statement. The code should print "The number is 5" when the number is 5, and should print "The number is NOT 5" when it is not.

            .. activecode::  ch12ex14q
                :nocodelens:

                x = 5
                if x == 5:
                print("The number is 5")
                if x != 5:
                print("The number is NOT 5")


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex14q

#.

    .. tabbed:: ch12ex15t

        .. tab:: Question

           Fix 5 errors in the following code to set price to 1.45 if weight is less than 1 and otherwise set it to 1.15.

           .. activecode::  ch12ex15q
                :nocodelens:

                weight = 0.5
                if weight < 1
                price = 1.45
                else
                price = 1.15
                total = weight * price
                print(weight)
                print(price
                print(Total)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex15q

#.

    .. tabbed:: ch12ex16t

        .. tab:: Question

            Complete and finish the code on lines 1 and 4 so that the code prints "Hi".

            .. activecode::  ch12ex16q
                :nocodelens:

                x =
                if not x != 3:
                    print("Hi")

                    print("Hello")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex16q

#.

    .. tabbed:: ch12ex17t

        .. tab:: Question

           Write a procedure that will print out "even" if the passed value is even and "odd" if the passed value is odd.  Test both possibilities.

           .. activecode::  ch12ex17q
                :nocodelens:

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex17q

#.

    .. tabbed:: ch12ex18t

        .. tab:: Question

            Write a procedure that takes 2 ints, total price, and amount in wallet. Print "You have enough money" if the difference between the wallet and price is 0 or greater; otherwise, print "Get more money"

            .. activecode::  ch12ex18q
                :nocodelens:

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex18q

#.

    .. tabbed:: ch12ex19t

        .. tab:: Question

           Write a function that takes a number for a grade and returns a string grade.  It should return E for any value below 60, D for 61 to 69, C for 70 to 79, B for 80 to 89 and A for 90 and above.  Write code to test each grade range.

           .. activecode::  ch12ex19q
               :nocodelens:

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex19q

#.

    .. tabbed:: ch12ex20t

        .. tab:: Question

            Write code that prints "Fizz" when the number is divisible by 3, "Buzz" when it is divisible by 5, and "FizzBuzz" when it is divisible by 3 and 5  (If a number is divisible by 3 and 5, it should also print "Fizz" and "Buzz").

            .. activecode::  ch12ex20q
                :nocodelens:


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch12ex20q
