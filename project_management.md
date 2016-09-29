
* Dossier partagé
	* R: AOCAIBRE
	* 3543 16 projman midterm


Exam final de deux heures avec 3 questions
1 question obligatoire sur les trois


# Introduction 15/09

> __Project__: a project is a collection of tasks, operations or activities that when completed constitute the end of the project. In general there a logical precedents rules between the activities.


_Example when building a house:_ 
* buying the site
* drawing the plans 
* planning applications
* excavation
* foundations

__Questions :__

1. What is the completion time for the project ? _(duration of the project)_  sometimes it's not possible to assign definite time to each activities but we must be able in this case to assign 3 possible times: [ Optimistic time; most likely time, and pessimistic time ]. In this case on most produce the expected project duration.
2. What resources are needed to complete the project in his completion time & is it possible to complete the project with fewer resources by delaying the start time on some activities. __This is called resources scheduling.__
3. What is the total cost of completing the project & is it possible to finish the project earlier and at what extra cost. __This is cost scheduling.__
4. In the case where each activities does not have a definite duration, then it is important to determine what is the probability that the project finishes by some specifies time ?

* PERT
	* __P__ rogram __E__ valuation __R__ eview and __T__ echnic
* CPA
	* __C__ ritical __P__ aram __A__ nalytic

>  __Network__ is a diagram made out of __nodes__ and __arrows__.

Node approach vs. arrow approach pour faire les networks afin de déterminer le temps nécessaire

* Node approach
	* On met les activités sur les __nodes__
* Arrow approach
	* On met les activités sur les __arrows__
* Each activity is represented my one arrow only
* Each arrow in the network __must__ represent an activity

> __The critical path__ is the longest path throw the network. It is the path that produces the project completion time.
> Need to flag the _critical path_ with flag on the arrow with this symbol: //
> There may be __many__ critical path all having there path time equal to the project duration.

Each activity on the critical path cannot be delayed without delaying the overall project time. This activities are called __critical activities__. _(in our case, A, E & G)_

> __FLOAT__ of an activities is the amount of the to start an activities can be delayed without affecting the overall project time.

# Resources scheduling
_In this section we want to determine the resources needed to complete the project in it's normal time._
 We can then exploit the float of certain activities to possibly complete the project with fewer resources. This can be achieved with a __block graph__ or a __GANTT chart__

* Block graph
	* Each activity represented by a block
		* Horizontal: activity time
		* Vertical: people required
	* __Always represent the critical path on the block graph first__
* GANTT chart

------
> Example of a project management with a __network__, a __FLOAT__ table and a __block graph__ to determine the time needed to achieve the project with some resources. 

![subject](http://i.imgur.com/r7uQIKw.jpg)
![solve](http://i.imgur.com/pF35ltV.jpg)

-------


> A __dummy activity__ is not an activity. ie: It require no time or resources but is absolutely necessary to satisfy the logical precedence rules. 



-----


Here is as example of _dummy activity_:

![Subject ](http://i.imgur.com/w4NI9HD.jpg)
![Answer](http://i.imgur.com/JpP16JQ.jpg)


----------



# PERT (Program Evaluation and Review Technic)

In reality, it is often not possible to assign definite or certain time for each activity to be completed. But it is also not unrealistic to put 3 possible values for each activities time. 
Theses are traditionally called: 

* Optimistic (__O__)
* Pessimistic (__P__)
* Most Likely (__ML__)

From this starting point one then creates an expected time for each activities together with the standard deviation of that __expected__ time.
This expected time and standard deviation are produced by the __PERT ESTIMATES__

`EXPECTED TIME = (O + 4 ML + P) / 6` 

`STANDARD DEVIATION = (P - O) / 6`


One having completed the network and determining the critical path one can now produce unexpected completion time for the project. Being unexpected time implies some uncertainty. Therefore, it is important to determine the probability that certain specifies paths may finish in some specified time.
For example what is the probability that the path CDFI finishes a day earlier in 29. This may be a useful piece of information.


# Normal distribution

Bell shaped symmetric curve
All normal distribution are all "the same" in the sense that the area under the curve some specified number of std deviation away from the center is always the same.