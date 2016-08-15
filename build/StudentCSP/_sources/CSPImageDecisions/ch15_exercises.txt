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
	:prefix: 15-6-

Chapter 15 Exercises
---------------------

Below is a selection of images that you can use in the programs in this section.

.. raw:: html

   <table>
   <tr><td>beach.jpg</td><td>baby.jpg</td><td>vangogh.jpg</td><td>swan.jpg</td></tr>
   <tr><td><img src="../_static/beach.jpg" id="beach.jpg"></td><td><img src="../_static/baby.jpg" id="baby.jpg"></td><td><img src="../_static/vangogh.jpg" id="vangogh.jpg"></td><td><img src="../_static/swan.jpg" id="swan.jpg"></td></tr>
   </table>
   <table>
   <tr><td>puppy.jpg</td><td>kitten.jpg</td><td>girl.jpg</td><td>motorcycle.jpg</td></tr>
   <tr><td><img src="../_static/puppy.jpg" id="puppy.jpg"></td><td><img src="../_static/kitten.jpg" id="kitten.jpg"></td><td><img src="../_static/girl.jpg" id="girl.jpg"></td><td><img src="../_static/motorcycle.jpg" id="motorcycle.jpg"></td></tr>
   </table>
   <table>
   <tr><td>gal1.jpg</td><td>guy1.jpg</td><td>gal2.jpg</td></tr>
   <tr><td><img src="../_static/gal1.jpg" id="gal1.jpg"></td><td><img src="../_static/guy1.jpg" id="guy1.jpg"></td><td><img src="../_static/gal2.jpg" id="gal2.jpg"></td></tr>
   </table>
   
   
.. note:: 

   Remember that it can take a bit of time to process all the pixels in a picture!  Check for errors below the code if it is taking a long time, but if you don't see any errors just wait.

#. 

    .. tabbed:: ch15ex1t

        .. tab:: Question
            
            Make changes to 10 lines in the code below so that it runs.  It changes areas that look red in the original to green.    

            .. activecode:: ch15ex1q
                :nocodelens:

                from  import *

                # CREATE AN IMAGE FROM A FILE
                img = Image("gal2.jpg")

                # LOOP THROUGH ALL PIXELS
                for x in range(img.getWidth()):
                    for y in range(img.getHeight())
                        p = img.getPixel(x, y)
                        r = p.getRed()
                        g = p.getGreen()
                        b = p.getBlue()

                    # VALUES FOR THE NEW COLOR
                    if r > 200 and g < 100 and b < 100:

                        # CREATE THE COLOR
                        newPixel = Pixel(0, g, b)

                        # CHANGE THE IMAGE
                        img.setPixel(x, y, newPixel)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img.getWidth(),img.getHeight())
                img.draw(win)
      	            
        
                
        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex1q

#. 

    .. tabbed:: ch15ex2t

        .. tab:: Question

           Fix the indention in the code below so that it runs correctly.  It does a primitive form of edge detection.
           
           .. activecode::  ch15ex2q
                :nocodelens:
                
                from image import *

                # CREATE AN IMAGE FROM A FILE
                img = Image("swan.jpg")

                # LOOP THROUGH ALL BUT LAST COLUMN
                for x in range(img.getWidth() - 1):
                    for y in range(img.getHeight()):
                    p = img.getPixel(x, y)
                    p2 = img.getPixel(x + 1, y)
                    r1 = p.getRed()
                    g1 = p.getGreen()
                    b1 = p.getBlue()
                    average1 = (r1 + g1 + b1) / 3
                    r2 = p2.getRed()
                    g2 = p2.getGreen()
                    b2 = p2.getBlue()
                    average2 = (r2 + g2 + b2) / 3

                    # VALUES FOR THE NEW COLOR
                    if abs(average2 - average1) > 10:
                    newPixel = Pixel(0, 0, 0)
                    else:
                    newPixel = Pixel(255, 255, 255)
                            
                        # CHANGE THE IMAGE
                        img.setPixel(x, y, newPixel)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img.getWidth(),img.getHeight())
                img.draw(win)
                
          
       
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex2q

#. 

    .. tabbed:: ch15ex3t

        .. tab:: Question

           Fix the indention in the code below so that it runs correctly.  It posterizes a picture which means that it reduces all the colors in a picture to a small number of colors – like the ones you might use if you were making a poster..
        
           .. activecode::  ch15ex3q
                :nocodelens:
                
                from image import *

                # CREATE AN IMAGE FROM A FILE
                img = Image("beach.jpg")

                # LOOP THROUGH ALL PIXELS
                for x in range(img.getWidth()):
                    for y in range(img.getHeight()):
                        p = img.getPixel(x, y)

                        r = p.getRed()
                        g = p.getGreen()
                        b = p.getBlue()

                        # VALUES FOR THE NEW COLOR
                        if r < 120:
                        r = 0
                        if r >= 120:
                        r = 120
                        if g < 120:
                        g = 0
                        if g >= 120:
                        g = 120
                        if b < 120:
                        b = 0
                        if b >= 120:
                        b = 120

                        # CREATE THE COLOR
                        newPixel = Pixel(r,g,b)

                        # CHANGE THE IMAGE
                        img.setPixel(x, y, newPixel)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img.getWidth(),img.getHeight())
                img.draw(win)

      


        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex3q
                
#. 
                
    .. tabbed:: ch15ex4t

        .. tab:: Question

           Fix 5 errors in the code below. It will copy the non-white pixels from gal1.jpg to guy1.jpg. 
           
           .. activecode::  ch15ex4q
                :nocodelens:

                from image import *

                # CREATE THE IMAGES
                img1 = Image("gal1.jpg")
                img2 = Image(guy1.jpg")

                # LOOP THROUGH ALL THE PIXELS IN IMG1
                for x in range(img1.getWidth():
                    for y in range(img1.getHeight())
                        p1 = img1.getPixel(x, )
                        r1 = p1.getRed()
                        g1 = p1.getGreen()
                        b1 = p1.getBlue()

                        # CHECK IF THE PIXEL ISN'T WHITE
                        if r1 < 250 and g1 < 250  b1 < 250:

                            # COPY THE COLOR TO IMG2
                            img2.setPixel(x, y, p1)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img2.getWidth(),img2.getHeight())
                img2.draw(win)


     
                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex4q
                

   
#. 

    .. tabbed:: ch15ex5t

        .. tab:: Question

           Change the code below to use ``if`` and ``else`` rather than two ``if`` statements per color.  It posterizes an image.
           
           .. activecode::  ch15ex5q
                :nocodelens:

                from image import *

                # CREATE AN IMAGE FROM A FILE
                img = Image("beach.jpg")

                # LOOP THROUGH ALL PIXELS
                for x in range(img.getWidth()):
                    for y in range(img.getHeight()):
                        p = img.getPixel(x, y)

                        r = p.getRed()
                        g = p.getGreen()
                        b = p.getBlue()

                        # VALUES FOR THE NEW COLOR
                        if r < 120:
                            r = 0
                        if r >= 120:
                            r = 120
                        if g < 120:
                            g = 0
                        if g >= 120:
                            g = 120
                        if b < 120:
                            b = 0
                        if b >= 120:
                            b = 120

                        # CREATE THE COLOR
                        newPixel = Pixel(r,g,b)

                        # CHANGE THE IMAGE
                        img.setPixel(x, y, newPixel)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img.getWidth(),img.getHeight())
                img.draw(win)

      

        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex5q
                
#. 

    .. tabbed:: ch15ex6t

        .. tab:: Question

           Change the following code into a procedure. It posterizes an image. Be sure to call it to test it.
           
           .. activecode::  ch15ex6q
                :nocodelens: 
                
                from image import *

                # CREATE AN IMAGE FROM A FILE
                img = Image("beach.jpg")

                # LOOP THROUGH ALL PIXELS
                for x in range(img.getWidth()):
                    for y in range(img.getHeight()):
                        p = img.getPixel(x, y)

                        r = p.getRed()
                        g = p.getGreen()
                        b = p.getBlue()

                        # VALUES FOR THE NEW COLOR
                        if r < 120:
                            r = 0
                        if r >= 120:
                            r = 120
                        if g < 120:
                            g = 0
                        if g >= 120:
                            g = 120
                        if b < 120:
                            b = 0
                        if b >= 120:
                            b = 120

                        # CREATE THE COLOR
                        newPixel = Pixel(r,g,b)

                        # CHANGE THE IMAGE
                        img.setPixel(x, y, newPixel)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img.getWidth(),img.getHeight())
                img.draw(win)
                
     

       
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex6q
                
#. 

    .. tabbed:: ch15ex7t

        .. tab:: Question

           Change the following into a procedure. It changes areas that are mostly red looking to green.  Be sure to call it to test it.
           
           .. activecode::  ch15ex7q
                :nocodelens: 
                
                from image import *

                # CREATE AN IMAGE FROM A FILE
                img = Image("gal2.jpg")

                # LOOP THROUGH ALL PIXELS
                for x in range(img.getWidth()):
                    for y in range(img.getHeight()):
                        p = img.getPixel(x, y)
                        r = p.getRed()
                        g = p.getGreen()
                        b = p.getBlue()

                        # VALUES FOR THE NEW COLOR
                        if r > 200 and g < 100 and b < 100:

                            # CREATE THE COLOR
                            newPixel = Pixel(0, g, b)

                            # CHANGE THE IMAGE
                            img.setPixel(x, y, newPixel)

                # SHOW THE CHANGED IMAGE
                win = ImageWin(img.getWidth(),img.getHeight())
                img.draw(win)
                
                

      
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex7q
                
#. 

    .. tabbed:: ch15ex8t

        .. tab:: Question

           Write the code to posterize a picture but use 3 values for each color instead of 2.  Use 0 if the current value is less than 85, use 85 if the value is less than 170, else use 170.
           
           .. activecode::  ch15ex8q
                :nocodelens:
                
                
      
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex8q
                
#. 

    .. tabbed:: ch15ex9t

        .. tab:: Question

           Write the code to do edge detection on a picture, but compare the curent pixel with the one below it rather than the one to the right. 
            
           .. activecode::  ch15ex9q
                :nocodelens:

       
                                
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex9q
                
#. 

    .. tabbed:: ch15ex10t

        .. tab:: Question

           Write a procedure to remove the red on very red pixels (pixels that have a red value greater than 200 and a green and blue value of less than 100).  
           
           .. activecode::  ch15ex10q
               :nocodelens:

       
         
                                 
        .. tab:: Discussion 

            .. disqus::
                :shortname: cslearn4u
                :identifier: studentcsp_ch15ex10q



