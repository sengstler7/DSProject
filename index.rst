.. DS 320 Project documentation master file, created by
   sphinx-quickstart on Mon Nov 26 22:32:53 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to DS 320 Project's documentation!
==========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

NHL API Game Data
+++++++++++++++++++++++
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

test


Plotting Goals vs Saves
+++++++++++++++++++++++++
Our first question was where certain goalies are more likely to give up goals from. The system we set up is interactive, but because of the limitations of this website, we were unable to port it over. Here is a map of Sergei Bobrovsky.

We can see that he tends to face a lot of shots close to the net, in the slot and in the crease. He tends to give up goals from those regions, as well as from shots near the blueline/point.

..figure:: Bob.png




Plotting Hits
++++++++++++++
Imaginary plot of hits



Im Still Testing the website
+++++++++++++++++++++++++

`In this notebook notebook

Plotting Face-offs
+++++++++++++++++++++
Imaginary plot of face-offs 


Interactive Charts!!
========================
Plots with interactive charts


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
