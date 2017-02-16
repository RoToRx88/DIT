[TOC]

#Opportunity lost **OL**
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
 