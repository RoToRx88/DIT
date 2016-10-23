
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

All number on the table of normal curve give the _"bigger half"_ and therefore sometimes you must substract from 1 to get the required aera.

> _Important fact about normal distribution_: 
> T he sum of normal distribution is again normal distribution with center equal to the sum of the centers and standard deviation equal to the square-root of the sum of the squares of standard deviations.



# Project Life Cycle

Project have typical the following 4 phases, each with it's own agenda of tasks & issues: 

* Initiation
* Planning
* Implementation
* Closure / End

## Initiation Phase

In this phase, the project objective is identified. This can be a business problem or opportunity. Most impotently issues of feasibility _(can we do the project)_, and justification _(should we do the project)_ are addressed. 

## Planning Phase

In this phase, the team identifies all the work that needs to be done. In particular the project tasks and resources requirement are identified along with the strategy for producing it. Finally a project plan is produced. Outlining the activities dependencies & time frames. A __network diagram__ is particularly useful in this phase. Once the project team has identified the work prepared the scheduled, estimated the cost, the 3 fundamentals components of the planning process are complete. It is also important in this phase to document providing insurances & control measures, quality target, along with an acceptance plan listing the criteria to gain customer acceptance.

## Implementation

In this phase project plan is put into motion and perform the work of the project.
It is very important in this phase to maintain control and communicate as needed. Progress is continuously monitored & as a result appropriate adjustments and made and recorded as variances from the original plan.
What's appen here is people are carrying tasks & progress information is beeing reported to regular teams meeting.
Finally, states reports should always emphasis the anticipated end point in terms of cost, scheduled & quality of deliverable. Each project deliverable produced should be reviewed for quality & measured against the acceptance criteria.

## Closure / End

In this final phase the emphasis is on releasing the final  deliverable to the customer in particular handing over project documentation to the customer terminating supplier contracts releasing resources & communicating the closure to all possible stakeholders.
The last remaining step is to conduct lessons learn studies _ie: to examine what went well and what did not_.
The resume of experiences is transferred back to the organisation which will have other project.

The technical term for the FLOAT calculate above is __TOTAL FLOAT__. There are 2 others types of float:

* FREE FLOAT
	* = EFT - EST - ACTIVITY TIME
		* EFT = EST start for subsequent activity
		* _ie: how much time the start of an activity can be delayed without affecting the EST of subsequent activities_
	*  
* INDEPENDENT FLOAT
	* = EST _(for subsequent)_ - LST _(for start act time)_


# Cost scheduling

In this section we are concerned with determining the cost of a project if it is completed in it _normal_ time (or _current_ time)

This cost is determined by adding up the cost for each activities when completed in it _normal_ or _current_ time. Some activities can be completed in a shorter time, but at an extra cost, usually per day. This is called the daily reduction cost (aka _cost slop_). Our final assumption is that there is a minimum time for each activities _ie: it can be reduced no further_. This time is called the __Crash Time__ and the cost associated with completing an activity in it's crash time is called the __Crash Cost__. The objective in this section is to determine the overall cost for completing a project in it's minimum time and comparing it with the cost of completing the project in it's normal time. _ie: is it beneficial to finish the project earlier than it's normal time_.


> __TODO__: Exercise n°8 + determine the FLOAT

> _crash (days)_: minimum amount of time takes an activity. 

The minimum possible project time is determined using the __crash time__ of each activity as follows:

1. crash every activity _ie: put the crash time for each activity in place of the current time on the network & determine all path time through the network & choose the maximum of this values_

The __crash time__ do give us the minimum project time but not the minimum cost associated with that time. It is not correct to add up the __crash cost__ for each activity to get this minimum cost because many activities have been crashed on necessarily. For example an activity with less crash time than the largest crash time is not necessary have to be done in his crash time, as it will induce extra cost. So don't crash every path, as it will add extra cost.

We now attempt to determine the minimum cost for the project.

1. Reduce the project time by 1 day. This is achieved by reducing one of the critical activities by 1 day because all other paths are less time than the critical path. We do this on the cheapest manner. _ie: the activity with the lowest daily reduction cost_ We continue to reduce until one of two obstacles appears. 1: the activity we are reducing crashes since no further reduction with that activity; 2: a new critical path appears. In this case the project time can only be reduced by reducing all critical paths. It is important at this stage to determine the float of each activities because project reduction will erase the float of some activities _ie: they will now become critical_
2.  