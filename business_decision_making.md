# Opportunity lost **OL**
> __Definition:__ This is the lost opportunity associated with making a decision.

When using an **opportunity lost** OL table, BAYES' rule now recommends making the decision with the lowest **expected** opportunity lost. _ie: in problem 2) stock 6._

There is also another rule for **OL** table called: **minimax rule**

> **Minimax**: take the best of the worth **OL** for each decision _ie in problem 2) stock 7._

## Perfect Information (Forecast) **PI**

The total of each decision of it's **expected payoff** and it's **expected opportunity lost** is always the same no mater what the decision. In the case of _problem 2)_ : 212
**Perfect Information** is the situation where (unrealistically) you have access to a perfect forecast for the different demand levels. The number _here in problem 2)_ 212 is called **Expected Payoff from Perfect Information** (EPPI)
From this value (EPPI), we can obtain something useful, called **EVPI** (**V** for Value / gain) as follows: take EPPI and subtract the best expected payoff in the payoff table _ie problem 2): 212 - 203.6 = 8.4; **EVPI** = 8.4_
EPPI always appear for free as the lowest expected opportunity (**pOL**) in the **OL** table.
This value **EVPI** gives us an upper limit on how much to pay for forecast in the long one.

# Probability (Bayesian) _aka: revising probability_

## Basics
1. 0 <= P(A) <= 1 means probability of a is included between 0 and 1
2. P(A) = 0 : A is impossible
3. P(A) = 1 : A is certain
4. P(A and B) = P(A) * P(B)
5. P(A or B) = P(A) + P(B) - P(A and B)
6. P(A | B) = probability of A occurring given that B occurring

## Problem 1

|  1000	|   High	|   Low	|   People out of 1000 that have +ive or -ive	|
|---	|---	|---	|---	|
|  +ive 	|  9 	|   99	|   108	|
|   -ive	|   1	|   891	|   	892|
|   People out pf 100 having High or Low	|  10 	|   990	|   	|

P(HIGH | +ive) = 9 / 108 = 0.083

Upon taking the test, the chances that a person shows positive is:
`P(+ive) = 108/1000 = 0.108`
within 108 people, 9 actually have high cholesterol
`P(HIGH | +ive) = 9 / 108 = 0.083`
This answer can be viewed in two opposites ways:

1. In absolute terms, 0.083 is a small probability therefore no need to worries
2. but in relative terms it is 8 times more likely than the original probability 0.01 (which is not a good things)

## Probability trees

The above problem can be solved with the **probability trees**

The tree structure is always started by the probability that is being revised.
_eg in the above problem: chance of high cholesterol 0.01; but once showing up positive this 0.01 was revised up to 0.083

   (i) P(+ive) = 0.009 + 0.99 = 0.108
(ii) P(High | +ive) = (0.009) / (0.009 + 0.099) = 0.083

**Insert Problem 3**
**Insert Problem 9**

**Insert Problem 15**

The above result is not very useful because it is said for every 100 persons who tested positive for steroïd use, just 16 were using steroid. In order to improve this test, we test again on someone who showed positive.
A person who shows up 2 time positive after 2 tests has a 64.4% chance of using steroids.

## Problem 15.1

The chances of having breast cancer and been tested positive on the mamograms is only 3% therefore the test is meaningless and this is why the government task force advice women in they 40's not to have annual mammograms.

## Problem 19

The above result suggest that 57% of rejected customers are potentially not defaulters _ie good customers_

In general all of theses problems fall under the following general scenario:
We start with a believe / probability that an event occurs _(ie problem #15.1 breast cancers, problem #19 not defaulting)_ then introduces new informations _(ie in #15.1 positive mammogram, in #19 reject)_ this then forces us to revise our initial believe based on that new information _(#15 0.04 was revised to 0.031 because of the positive mammogram; #19 0.8 vvas revised down to 0.57 because of the rejection)_

## Problem 11

Initially 60% of disputes over wages but once we have the new information that it is resolved without a strike, we must revise that 60% down to 56.8%.


# Decision Trees

In payoff tables, we would dealing with the decision making problems where the decisions options were identicals to the actual demand options. _ie stock 4, 5, 6 or 7, and demand can be 4, 5, 6 or 7. We now generalize to the situation where the decisions options are not the same as the demand posibilities.

## Problem 2

The above tree structure represent deciding between choice A1 and A2 _(ie the boxe)_, but once having make that choice, 3 events can occure _(out of your control, represented by a circle node)_. In the above tree, 3 events can occure once having made your choice. Theses events are E1, E2, E3.

We now apply base rule named make the decision with the greatest expected value _ie the value for node 1_ which implies choose A1 ie skimming price strategy.
MaxiMax: A1
MaxiMin: A2
MiniMax: A1

## Problem 2 v2.

it is not correct to put the probabilities 0.2 0.6 0.2 (exo 2b) because one's given a favorable result from the research this will force us to revise the probabilities for E1, E2 and E3. The revised probability for E3 will go up, while E1 will go down if the research is favorable. Similarly if the result of the research is unfavorable, then the probability of E1 will go up, and E3 will go down. These revised probabilities are now determined using the following probability tree.

THe above value (11.2225) is the expected value from the reasearch, with no fees, we mumst now include the fee to get : `expected_value_of_doing_research - 0.5 = 11.2225 - 0.5 = 10.7225 < 11 millions`
So __don't__ do research

_ie no research: choose A1, expected profit 11 millions_

The reason for not doing research is it is too expensive. For example, the
expected return for doing research no fee is 11.2225m€. Therefore if the
researcher charges less than 0.2225m€ (11.2225 - 11) then he is worth it. We
call this value 0.2225 __the expected value of the reserach information__. In
summury if the researcher charged less than the expected value of information,
then they would be worth it.
