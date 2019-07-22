..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".

.. 	qnum::
	:start: 1
	:prefix: csp-18-8-

Finding the Pollution for a State
===================================

We can use **split** to chop up our data by fields, separated by ":".  But we can also use it *within*  field, to separate by space.  If we split the city/state by "space", we'd get city and state as two different elements of the list.

This section uses the same data file that we have been using, but if you want to see **all** of the data click on the *Show* button below.  Once it appears, you can hide it again by clicking on the *Hide* button.

.. reveal:: pol_Data_7
    :showtitle: Show
    :hidetitle: Hide

    .. raw:: html

       <pre id="uspoll.txt">
       Aberdeen, SD :13 :8
       Adrian, MI :15 :9
       Akron, OH :18 :11
       Albany, GA :18 :11
       Albany-Lebanon, OR :14 :8
       Albany-Schenectady-Troy, NY :13 :8
       Albuquerque, NM :12 :7
       Alexandria, LA :20 :12
       Allegan, MI :14 :9
       Allentown-Bethlehem-Easton, PA-NJ :21 :12
       Altoona, PA :19 :12
       Anchorage, AK :13 :8
       Anderson, IN :18 :11
       Ann Arbor, MI :16 :10
       Appleton, WI :14 :9
       Asheville, NC :15 :9
       Athens, OH :14 :9
       Athens, TN :15 :9
       Athens-Clarke County, GA :16 :9
       Atlanta-Sandy Springs-Marietta, GA :23 :14
       Atlantic City-Hammonton, NJ :14 :8
       Augusta-Richmond County, GA-SC :18 :11
       Augusta-Waterville, ME :14 :9
       Austin-Round Rock, TX :17 :10
       Bakersfield, CA :24 :15
       Baltimore-Towson, MD :20 :12
       Bangor, ME :12 :7
       Baraboo, WI :17 :10
       Baton Rouge, LA :19 :11
       Bay City, MI :13 :8
       Beaver Dam, WI :15 :9
       Beckley, WV :14 :8
       Bellingham, WA :7 :4
       Bennington, VT :11 :7
       Birmingham-Hoover, AL :20 :12
       Bishop, CA :11 :6
       Bismarck, ND :11 :6
       Bloomington, IN :17 :10
       Bloomington-Normal, IL :16 :9
       Boise City-Nampa, ID :17 :10
       Boone, NC :13 :8
       Boston-Cambridge-Quincy, MA-NH :16 :10
       Boulder, CO :12 :7
       Bowling Green, KY :17 :10
       Bradenton-Sarasota-Venice, FL :12 :7
       Brainerd, MN :8 :5
       Bremerton-Silverdale, WA :7 :4
       Bridgeport-Stamford-Norwalk, CT :16 :9
       Brigham City, UT :12 :7
       Brookings, SD :14 :9
       Brownsville-Harlingen, TX :16 :10
       Brunswick, GA :13 :8
       Buffalo-Niagara Falls, NY :16 :9
       Burlington, NC :14 :9
       Burlington-South Burlington, VT :12 :7
       Butte-Silver Bow, MT :19 :11
       Cadillac, MI :10 :6
       Cambridge, MD :13 :8
       Canton-Massillon, OH :21 :12
       Cape Coral-Fort Myers, FL :12 :7
       Casper, WY :9 :5
       Cedar Rapids, IA :16 :10
       Champaign-Urbana, IL :16 :10
       Charleston, WV :18 :11
       Charleston-North Charleston-Summerville, SC :16 :10
       Charlotte-Gastonia-Concord, NC-SC :16 :10
       Charlottesville, VA :13 :8
       Chattanooga, TN-GA :18 :11
       Cheyenne, WY :9 :6
       Chicago-Naperville-Joliet, IL-IN-WI :22 :13
       Chico, CA :12 :7
       Cincinnati-Middletown, OH-KY-IN :23 :14
       Clarksburg, WV :16 :10
       Clarksville, TN-KY :16 :10
       Clearlake, CA :7 :4
       Cleveland-Elyria-Mentor, OH :24 :15
       Clinton, IA :18 :11
       Colorado Springs, CO :12 :7
       Columbia, SC :17 :10
       Columbia, TN :14 :8
       Columbus, GA-AL :19 :11
       Columbus, OH :18 :11
       Concord, NH :16 :9
       Cookeville, TN :14 :9
       Corning, NY :11 :7
       Corpus Christi, TX :18 :11
       Dallas-Fort Worth-Arlington, TX :20 :12
       Daphne-Fairhope-Foley, AL :15 :9
       Davenport-Moline-Rock Island, IA-IL :18 :11
       Dayton, OH :18 :11
       Decatur, AL :15 :9
       Decatur, IL :17 :10
       Deltona-Daytona Beach-Ormond Beach, FL :11 :6
       Denver-Aurora-Broomfield, CO :14 :9
       Des Moines-West Des Moines, IA :15 :9
       Detroit-Warren-Livonia, MI :21 :12
       Dickinson, ND :7 :4
       Dothan, AL :15 :9
       Dover, DE :14 :8
       Duluth, MN-WI :11 :6
       Durango, CO :7 :4
       Durham, NC :14 :8
       Durham-Chapel Hill, NC :14 :8
       Dyersburg, TN :15 :9
       East Stroudsburg, PA :13 :8
       Eau Claire, WI :14 :8
       El Centro, CA :24 :14
       El Dorado, AR :18 :11
       El Paso, TX :21 :12
       Elizabethtown, KY :20 :12
       Elkhart-Goshen, IN :21 :12
       Erie, PA :19 :11
       Eugene-Springfield, OR :13 :8
       Eureka-Arcata-Fortuna, CA :11 :7
       Evansville, IN-KY :19 :12
       Fairbanks, AK :31 :19
       Fairmont, WV :17 :10
       Fargo, ND-MN :13 :8
       Farmington, NM :8 :5
       Fayetteville, NC :15 :9
       Fayetteville-Springdale-Rogers, AR-MO :16 :10
       Flagstaff, AZ :9 :5
       Flint, MI :13 :8
       Florence, SC :15 :9
       Florence-Muscle Shoals, AL :15 :9
       Fort Collins-Loveland, CO :12 :7
       Fort Madison-Keokuk, IA-MO :18 :11
       Fort Payne, AL :15 :9
       Fort Smith, AR-OK :17 :10
       Fort Wayne, IN :23 :14
       Fresno, CA :74 :45
       Gadsden, AL :16 :10
       Gainesville, FL :12 :7
       Gainesville, GA :16 :9
       Gettysburg, PA :18 :11
       Gillette, WY :13 :8
       Goldsboro, NC :21 :13
       Grand Island, NE :13 :8
       Grand Junction, CO :12 :7
       Grand Rapids-Wyoming, MI :16 :10
       Grants Pass, OR :12 :7
       Greeley, CO :13 :8
       Green Bay, WI :16 :10
       Greensboro-High Point, NC :14 :9
       Greenville, NC :13 :8
       Greenville-Mauldin-Easley, SC :16 :10
       Grenada, MS :16 :9
       Gulfport-Biloxi, MS :16 :10
       Hagerstown-Martinsburg, MD-WV :19 :11
       Hammond, LA :15 :9
       Hanford-Corcoran, CA :28 :17
       Harriman, TN :22 :13
       Harrisburg-Carlisle, PA :20 :12
       Harrisonburg, VA :15 :9
       Hartford-West Hartford-East Hartford, CT :14 :9
       Hattiesburg, MS :18 :11
       Helena, MT :16 :9
       Helena-West Helena, AR :16 :9
       Hickory-Lenoir-Morganton, NC :16 :10
       Hilo, HI :27 :16
       Hobbs, NM :13 :8
       Holland-Grand Haven, MI :15 :9
       Homosassa Springs, FL :11 :7
       Honolulu, HI :12 :7
       Hot Springs, AR :18 :11
       Houma-Bayou Cane-Thibodaux, LA :13 :8
       Houston-Sugar Land-Baytown, TX :21 :13
       Huntington-Ashland, WV-KY-OH :19 :11
       Huntsville, AL :16 :9
       Indianapolis-Carmel, IN :25 :15
       Iowa City, IA :16 :10
       Jackson, MS :19 :11
       Jackson, TN :15 :9
       Jackson, WY-ID :11 :6
       Jacksonville, FL :13 :8
       Jamestown-Dunkirk-Fredonia, NY :13 :8
       Jasper, IN :18 :11
       Johnstown, PA :19 :12
       Juneau, AK :11 :6
       Kahului-Wailuku, HI :11 :6
       Kalamazoo-Portage, MI :17 :10
       Kalispell, MT :13 :8
       Kansas City, MO-KS :24 :15
       Kapaa, HI :11 :7
       Keene, NH :16 :10
       Kingsport-Bristol-Bristol, TN-VA :15 :9
       Kinston, NC :13 :8
       Klamath Falls, OR :18 :11
       Knoxville, TN :18 :11
       Kokomo, IN :16 :10
       La Crosse, WI-MN :14 :8
       Laconia, NH :11 :7
       Lafayette, IN :24 :14
       Lafayette, LA :18 :11
       Lake Charles, LA :14 :8
       Lake Havasu City-Kingman, AZ :6 :4
       Lakeland-Winter Haven, FL :13 :8
       Lancaster, PA :21 :13
       Lansing-East Lansing, MI :14 :9
       Laramie, WY :9 :6
       Las Cruces, NM :25 :15
       Las Vegas-Paradise, NV :20 :12
       Laurel, MS :18 :11
       Lawrenceburg, TN :14 :8
       Lebanon, NH-VT :11 :7
       Lebanon, PA :24 :14
       Lewiston-Auburn, ME :13 :8
       Lexington-Fayette, KY :16 :10
       Lima, OH :17 :10
       Lincoln, NE :14 :9
       Little Rock-North Little Rock-Conway, AR :19 :12
       Logan, UT-ID :15 :9
       Los Angeles-Long Beach-Santa Ana, CA :33 :20
       Louisville/Jefferson County, KY-IN :22 :13
       Lumberton, NC :14 :9
       Lynchburg, VA :13 :8
       Macon, GA :19 :12
       Madera, CA :27 :16
       Madison, WI :16 :9
       Manchester-Nashua, NH :14 :8
       Marshall, MN :12 :7
       Marshall, TX :17 :10
       McAlester, OK :19 :11
       McAllen-Edinburg-Mission, TX :18 :11
       Medford, OR :15 :9
       Memphis, TN-MS-AR :17 :10
       Merced, CA :18 :11
       Meridian, MS :17 :10
       Miami-Fort Lauderdale-Pompano Beach, FL :14 :8
       Michigan City-La Porte, IN :16 :10
       Middlesborough, KY :17 :10
       Milwaukee-Waukesha-West Allis, WI :18 :11
       Minneapolis-St. Paul-Bloomington, MN-WI :17 :10
       Missoula, MT :21 :12
       Mobile, AL :15 :9
       Modesto, CA :25 :15
       Monroe, LA :22 :13
       Monroe, MI :16 :9
       Montgomery, AL :18 :11
       Morgantown, WV :15 :9
       Mount Vernon, IL :14 :9
       Muncie, IN :16 :10
       Muscatine, IA :18 :11
       Muskegon-Norton Shores, MI :15 :9
       Napa, CA :23 :14
       Nashville-Davidson--Murfreesboro--Franklin, TN :17 :10
       New Castle, IN :15 :9
       New Haven-Milford, CT :15 :9
       New Orleans-Metairie-Kenner, LA :21 :13
       New York-Northern New Jersey-Long Island, NY-NJ-PA :23 :14
       Niles-Benton Harbor, MI :14 :9
       Nogales, AZ :16 :10
       Norwich-New London, CT :13 :8
       Ogden-Clearfield, UT :15 :9
       Oklahoma City, OK :16 :10
       Omaha-Council Bluffs, NE-IA :19 :12
       Orlando-Kissimmee, FL :12 :7
       Owensboro, KY :18 :11
       Oxnard-Thousand Oaks-Ventura, CA :16 :10
       Paducah, KY-IL :17 :10
       Palm Bay-Melbourne-Titusville, FL :10 :6
       Parkersburg-Marietta-Vienna, WV-OH :17 :10
       Pascagoula, MS :15 :9
       Pendleton-Hermiston, OR :12 :7
       Pensacola-Ferry Pass-Brent, FL :14 :8
       Peoria, IL :16 :10
       Philadelphia-Camden-Wilmington, PA-NJ-DE-MD :28 :17
       Phoenix-Mesa-Scottsdale, AZ :26 :16
       Pittsburgh, PA :25 :15
       Pittsfield, MA :14 :9
       Platteville, WI :15 :9
       Pocatello, ID :15 :9
       Ponca City, OK :17 :10
       Portland-South Portland-Biddeford, ME :15 :9
       Portland-Vancouver-Beaverton, OR-WA :12 :7
       Portsmouth, OH :16 :10
       Poughkeepsie-Newburgh-Middletown, NY :13 :8
       Prescott, AZ :7 :4
       Prineville, OR :14 :9
       Providence-New Bedford-Fall River, RI-MA :18 :11
       Provo-Orem, UT :14 :8
       Pueblo, CO :11 :7
       Quincy, IL-MO :16 :10
       Raleigh-Cary, NC :16 :9
       Rapid City, SD :11 :6
       Reading, PA :19 :11
       Red Bluff, CA :14 :8
       Redding, CA :10 :6
       Reno-Sparks, NV :15 :9
       Richmond, VA :15 :9
       Richmond-Berea, KY :15 :9
       Riverside-San Bernardino-Ontario, CA :34 :21
       Riverton, WY :13 :8
       Roanoke, VA :15 :9
       Rochester, MN :13 :8
       Rochester, NY :14 :9
       Rock Springs, WY :13 :8
       Rockford, IL :16 :9
       Rocky Mount, NC :13 :8
       Rome, GA :18 :11
       Russellville, AR :14 :9
       Rutland, VT :15 :9
       Sacramento--Arden-Arcade--Roseville, CA :15 :9
       Salinas, CA :10 :6
       Salisbury, NC :16 :9
       Salt Lake City, UT :15 :9
       San Antonio, TX :14 :9
       San Diego-Carlsbad-San Marcos, CA :24 :14
       San Francisco-Oakland-Fremont, CA :16 :10
       San Jose-Sunnyvale-Santa Clara, CA :16 :10
       San Luis Obispo-Paso Robles, CA :16 :10
       Santa Barbara-Santa Maria-Goleta, CA :14 :9
       Santa Cruz-Watsonville, CA :10 :6
       Santa Fe, NM :8 :5
       Santa Rosa-Petaluma, CA :14 :8
       Sault Ste. Marie, MI :14 :8
       Savannah, GA :17 :10
       Scottsbluff, NE :9 :6
       Scranton--Wilkes-Barre, PA :14 :8
       Seaford, DE :14 :8
       Seattle-Tacoma-Bellevue, WA :16 :10
       Sheridan, WY :14 :8
       Shreveport-Bossier City, LA :26 :16
       Sierra Vista-Douglas, AZ :11 :7
       Sioux City, IA-NE-SD :16 :10
       Sioux Falls, SD :14 :9
       Somerset, KY :16 :10
       South Bend-Mishawaka, IN-MI :21 :13
       Spartanburg, SC :16 :10
       Spokane, WA :12 :7
       Springfield, IL :16 :10
       Springfield, MA :15 :9
       Springfield, MO :17 :10
       Springfield, OH :17 :10
       St. Cloud, MN :14 :8
       St. George, UT :11 :7
       St. Joseph, MO-KS :20 :12
       St. Louis, MO-IL :22 :13
       State College, PA :19 :11
       Stockton, CA :21 :12
       Syracuse, NY :12 :7
       Talladega-Sylacauga, AL :17 :10
       Tallahassee, FL :14 :9
       Tampa-St. Petersburg-Clearwater, FL :13 :8
       Terre Haute, IN :19 :12
       Texarkana, TX-Texarkana, AR :18 :11
       Thomasville-Lexington, NC :17 :10
       Toledo, OH :17 :10
       Topeka, KS :14 :9
       Torrington, CT :9 :6
       Trenton-Ewing, NJ :15 :9
       Truckee-Grass Valley, CA :10 :6
       Tucson, AZ :10 :6
       Tulsa, OK :16 :10
       Tupelo, MS :16 :10
       Tuscaloosa, AL :16 :9
       Ukiah, CA :12 :7
       Valdosta, GA :14 :9
       Vallejo-Fairfield, CA :15 :9
       Vernal, UT :12 :7
       Virginia Beach-Norfolk-Newport News, VA-NC :14 :8
       Visalia-Porterville, CA :25 :15
       Warner Robins, GA :16 :10
       Washington-Arlington-Alexandria, DC-VA-MD-WV :19 :12
       Waterloo-Cedar Falls, IA :16 :10
       Watertown, SD :18 :11
       Weirton-Steubenville, WV-OH :20 :12
       Wenatchee, WA :17 :10
       Wheeling, WV-OH :20 :12
       Wichita, KS :16 :9
       Wilmington, NC :14 :9
       Winchester, VA-WV :16 :10
       Winston-Salem, NC :15 :9
       Worcester, MA :15 :9
       Yakima, WA :17 :10
       York-Hanover, PA :20 :12
       Youngstown-Warren-Boardman, OH-PA :23 :14
       Yuba City, CA :12 :7
       Yuma, AZ :14 :9
       </pre>

.. activecode:: splitCityState
   :tour_1: "Line-by-line tour"; 1: state1-line1; 2: state1-line2; 3: state1-line3; 4: state1-line4; 5: state1-line5; 6: state1-line6; 7: state1-line7;

   line = "Yuma, AZ :14 :9"
   pieces = line.split(":")
   print("All the pieces:")
   print(pieces)
   cityState = pieces[0].split(" ")
   print("City:", cityState[0])
   print("State:", cityState[1])
   print("PM 10:", pieces[1])
   print("PM 2.5:", pieces[2])

But, what if the city name has a space in it?  Then we won't get the state in the second slot.  It is safer to split on ``,``.

.. activecode:: splitCityState2
   :tour_1: "Line-by-line tour"; 1: state2-line1; 2: state2-line2; 3: state2-line3; 4: state2-line4; 5: state2-line5; 6: state2-line6; 7: state2-line7;

   line = "Yuba City, CA :12 :7"
   pieces = line.split(":")
   print("All the pieces:")
   print(pieces)
   cityState = pieces[0].split(",")
   print("City:", cityState[0])
   print("State:", cityState[1])

So, to check for particular state, we want to know if the current state name *matches* the one we're looking for.  We can use the ``strName.find(test)`` function to see if the current state is the one we are looking for.  The ``find`` function returns the index of the ``test`` in ``strName`` or -1 if it isn't found.

Now, let's reuse the average code and look for a particular state.

.. activecode:: average25state
   :tour_1: "Structural tour"; 2-4: state3-line1-3; 7-9: state3-line5-7; 12: state3-line8; 15: state3-line9; 18: state3-line10; 21: state3-line11; 24: state3-line12; 25: state3-line13; 28: state3-line14; 31: state3-line16;
   :nocodelens:

   # read all the lines
   infile = open("uspoll.txt","r")
   lines = infile.readlines()
   infile.close()

   # initialize the variables
   state = "CA"
   total25 = 0
   count = 1.0

   # loop through the lines
   for line in lines:

       # split at :
       values = line.split(":")

       # split at ,
       cityState = values[0].split(",")

       # if found state
       if cityState[1].find(state) >= 0:

           # add the current to the sum
           new25 = float(values[2])
           total25 = total25 + new25

           # increment the count
           count = count + 1

   # print the average
   print("Average PM 2.5 value for " , state, " is ", total25/count)

Use the below active code area to figure out the PM 10 code.  Replace the lines that start with ``#``.

.. activecode:: average10state
   :nocodelens:

   infile = open("uspoll.txt","r")
   lines = infile.readlines()
   infile.close()

   state = "CA"
   # create and initialize total10
   count = 1.0
   for line in lines:
       values = line.split(":")
       cityState = values[0].split(",")
       if cityState[1].find(state) >= 0:
           # get the current pollution value
           # add the current pollution to total10
           count = count + 1

   print("Average PM 10 value for ", state, " is ", total10/count)

What states have the highest average pollution values?  What do you think is most related to pollution: Population, area, or wealth?  Does it differ by PM 2.5 and PM 10?  For a list of the state two-letter abbreviations see http://www.50states.com/abbreviations.htm#.VJCB9r5NsXc.

.. parsonsprob:: 18_8_1_avg25
   :numbered: left
   :adaptive:

   The following program prints the average PM 2.5 pollution for a state, but the code is mixed up. Drag the blocks of statements from the left column to the right column and put them in the right order.  Then click on <i>Check Me</i> to see if you are right. You will be told if any of the lines are in the wrong order or have the wrong indention.
   -----
   # read all the lines
   infile = open("uspoll.txt","r")
   lines = infile.readlines()
   infile.close()

   # initialize the variables
   state = "CA"
   total25 = 0
   count = 1.0
   =====
   # loop through the lines
   for line in lines:
   =====
       # split at :
       values = line.split(":")
   =====
       # split at ,
       cityState = values[0].split(",")
   =====
       # if found state
       if cityState[1].find(state) >= 0:
   =====
           # add the current to the sum
           new25 = float(values[2])
           total25 = total25 + new25

           # increment the count
           count = count + 1
   =====
   # print the average
   avg = total25/count
   print("Avg for " , state, " is ", avg)

.. note::

    Discuss topics in this section with classmates.

      .. disqus::
          :shortname: cslearn4u
          :identifier: studentcsp_18_8
