.. 	qnum::
	:start: 1
	:prefix: 16-11-

Mixed Up Code Practice
------------------------------

.. parsonsprob:: ch16ex1muc
   :numbered: left
   :adaptive:
   :noindent:

   The following program segment should swap the first and last values of the list "numbers" using indexing. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   numbers = [3, 2, 1, 4]
   =====
   first = numbers[0]
   last = numbers[3]
   =====
   numbers[0] = last
   numbers[-1] = first
   =====
   first = numbers[1]
   last = numbers[4] #distractor


.. parsonsprob:: ch16ex2muc
   :numbered: left
   :adaptive:

   The following program segment should iterate through the list of prices and discount them by 50%. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   prices <- [21.99, 25.99, 19.99, 10.99, 15.99]
   discounts <- []
   =====
   FOR EACH price IN prices
   =====
       new_price <- price * .50
   =====
       APPEND(discounts, new_price)
   =====
   FOR EACH price IN discounts #distractor
   =====
       APPEND(price, prices) #distractor


.. parsonsprob:: ch16ex3muc
   :numbered: left
   :adaptive:

   The following program segment should iterate through the strings in list and append them to long_list if the length is greater than 4. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>

   -----
   list = ["four", "Michigan", "yellow", "at", "blue"]
   long_list = []
   =====
   for each item in list:
   =====
       if len(item) > 4:
   =====
           long_list.append(item)
   =====
           item.append(long_list) #distractor


.. parsonsprob:: ch16ex4muc
   :numbered: left
   :adaptive:

   The following program segment should first replace the last item of the list "months" with "November" then append "December" to the end of the list. But, the blocks have been mixed up and include extra blocks that aren't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   months = ["January", "March", "June", "August", "October"]
   new_month = "November"
   =====
   for word in terms:
   =====
   months.append("December")
   =====
   months[5] = new_month #distractor
   =====
   months[-1] = "December" #distractor


.. parsonsprob:: ch16ex5muc
   :numbered: left
   :adaptive:

   The following program segment should iterate through the list "terms" and then add each item to the list "vocab" if it is not already in the list. If the word is already in "vocab", then the program should add 1 to the variable "counter". But the blocks have been mixed up and include extra blocks that aren't needed in the solution. Drag the needed blocks from the left and put them in the correct order on the right. Click the <i/>Check Me</i> button to check your solution.</p>
   -----
   terms = ["accent", "vertigo", "libra", "illusion"]
   vocab = ["hereditary", "illusion", "vertigo", "velocity", "fallacy"]
   counter = 0
   =====
   for word in terms:
   =====
       if word NOT in vocab:
   =====
           vocab.append(word)
   =====
           word.append(vocab) #distractor
   =====
       if word in vocab:
   =====
           counter += 1
   =====
           counter + 1 #distractor