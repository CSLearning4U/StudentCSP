.. 	qnum::
	:start: 1
	:prefix: 17-10-

Mixed Up Code Practice
------------------------------

.. parsonsprob:: ch17ex1muc
   :numbered: left
   :practice: T
   :adaptive:
   :noindent:

   The following program segment should split the string "phrase" by each word and assign it to variable "x". Then insert the word into the string "final" and print the result.  But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   phrase = "Who did Jordan play against?"
   =====
   x = phrase.split(" ")
   =====
   x = split(phrase) #distractor
   =====
   name = x[2]
   =====
   name = x[3] #distractor
   =====
   final = name + "is his name."
   =====
   print(final)


.. parsonsprob:: ch17ex2muc
   :numbered: left
   :practice: T
   :adaptive:
   :noindent:

   The following program segment should print the integers in order <i>4, 9, 12</i> using the find function. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
   -----
   sent = "The girl was going home."
   =====
   num = str.find("girl")
   =====
   print(num) #paired
   =====
   num = str.find("going") #distractor
   =====
   print(num) #paired
   =====
   x = str.find("was")
   =====
   print(x) #paired
   =====
   x = str.find("as") #distractor
   =====
   print(x) #paired
   =====
   y = str.find(" going")
   =====
   print(y) #paired
   =====
   y = str.find("home") #distractor
   =====
   print(y) #paired


.. parsonsprob:: ch17ex3muc
  :numbered: left
  :practice: T
  :adaptive:
  :noindent:

  The following program segment should take the name from <i>sent_1</i> and assign it to the variable <i>first_name</i> using indexing. Then add the string to the variable <i>last_name</i> to create the variable <i>full_name</i>. Finally, add <i>full_name</i> to the <i>favorite</i> and print the result. But, the blocks have been mixed up and include an extra block that isn't needed in the solution.  Drag the needed blocks from the left and put them in the correct order on the right.  Click the <i>Check Me</i> button to check your solution.</p>
  -----
  sent_1 = "When Jimi got here, there was a commotion."
  last_name = " Hendrixx"
  =====
  first_name = sent_1[5:9]
  =====
  first_name = sent_1[5:8] #distractor
  =====
  full_name = first_name + last_name
  =====
  favorite = full_name + " is my favorite artist!"
  =====
  favorite = full_name + is my favorite artist! #distractor
  =====
  print(favorite)