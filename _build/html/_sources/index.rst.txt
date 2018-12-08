.. DS 320 Project documentation master file, created by
   sphinx-quickstart on Mon Nov 26 22:32:53 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to DS 320 Project's documentation!
===========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

NHL API Game Data
++++++++++++++++++++++++
.. figure:: https://cohenconnect.files.wordpress.com/2018/02/nhl-logo.png

Our project uses the NHL API to plot on ice locations for various types of plays that have happened so far this season. 
`Click here to view the NHL API <https://github.com/erunion/sport-api-specifications/tree/master/nhl>`_

We were able to scrape every game so far this season and break down every interesting play. We took the data we got and broke it down into these columns:
'Game_id'
'Event_idx', 'Period'
'Period_Time'
'Period_Time_Remaining'
'Period_Type'
'Event'- 'Faceoff','Hit','Shot','Giveaway','Missed Shot','Blocked Shot','Takeaway','Goal','Penalty'
'Xer' – The person performing the action
'Xer_id'
'Xer_team'
'Xee' – The person having the action done on them
'Xee_id'
'Xee_team'
'tx' -True Y value
'ty' -True Y value
'ax' -Halfsheet adjusted x
'ay' - Halfsheet adjusted y
'Secondary_Type' -Shot type on shots and goals, penalty type on penalties
'Pen_Min' – penalty minutes
'Ass1' -Assist1
'Assid1'
'Ass2' -Assist2
'Assid2'
'Strength' -powerplay even or shorthanded
"EN" -True or False if the goal was into an empty net




Plotting Goals vs Saves
++++++++++++++++++++++++++
Our first question was where certain goalies are more likely to give up goals from. The system we set up is interactive, but because of the limitations of this website, we were unable to port it over. Here is a map of Sergei Bobrovsky.

We can see that he tends to face a lot of shots close to the net, in the slot and in the crease. He tends to give up goals from those regions, as well as from shots near the blueline/point.

.. figure:: Bob.png




Hardest Worker
++++++++++++++++++
For our next visualization we created deals with who on the ice is the hardest worker. We took players based on the number of times they appeared as 'Xer' or 'Xee' and added them together.

.. figure:: HarderWorkingPlayerDistrubtion.png

Like most sport stat distributions, this plot is heavily skewed. Because all of our plots had the same issue with the skewness, we decided that it would be more interesting to highlight a few specific players and see what they do best.


Hardest Working Player
+++++++++++++++++++++++++
We can see in black the hits he takes and gives around the boards, the shots he has blocked and blocks in pink,and the shots and goals in blue and green. He seems to have a lot of ‘dump ins’ or shots from the blue line, and takes a lot of abuse in the corners.

.. figure:: BoHorvat.png


Most Effetive Player
+++++++++++++++++++++
For the most effective worker, we took the number of times that person was the Xer and divided it by the number of times they were the Xee. The most effective by our measure was Rasmus Ristolainen:
His graph looks very similar to Bo Horvat's, but with more blocked shots and hits. This makes sense as Ristolainen is a defender, while Horvat plays as a center.
.. figure:: Risto.png 


Most Goals
+++++++++++
This chart is the location of all the shots (blue) and goals(green) that Winnipeg Jets forward Patrik Laine has taken this season.

.. figure:: Laine.png

Most Blocked Shots
+++++++++++++++++++++
Ian Cole, a defender for the Pittsburgh Penguins takes the crown as the player with the most blocked shots this season. It makes sense that most of his blocks are clustered right in front of the crease, as a defender its his job to protect the net.

.. figure:: IanCole.png


Most Take-aways
++++++++++++++++
Florida Panthers' forward Aleksander Barkov is the NHL's take-away king. As a center, he is required to be more defensively responsible than his two wings. 

.. figure:: Barkov.png


Most Give-aways
+++++++++++++++++
On the other end of the spectrum we have the player with the most give-aways. Somewhat surprisingly this player is Drew Doughty, an all-star defenseman for the Los Angeles Kings.

.. figure:: Doughty.png


Biggest Hitter
+++++++++++++++
Hockey is a contact sport, and William Carrier of the Vegas Golden Knights is a perfect example of that. Carrier is leading the NHL in hits this season, and is on pace to break the record for most hits recorded in a season. 

.. figure:: Carrier.png


Least Disciplined
++++++++++++++++++
However, some players cross the line with their play. Whether it be through stick infractions or dangerous hits, players do need to serve their time in the penalty box if they make a mistake. Evander Kane, however has had a tough time learning his lesson, leading the NHL in penalties taken this season.

.. figure:: EvanderKane.png


Summary
++++++++
There is a lot of potential in this dataset to create in depth scouting reports for players and teams. Our Data Visualisations are on the beginning of what you can find using the NHL's API, and with the world of hockey changing very quickly, there is always more work to be done when analysing players.



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
