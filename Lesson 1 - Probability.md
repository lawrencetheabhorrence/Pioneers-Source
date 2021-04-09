---
title: Lesson 1
subtitle: Probability
date: March 28, 2020
header-includes: |
  \include{amsmath}
---

# Probability
Probability, informally, is the chances of an event happening, represented as a number between 0 and 1. A probability of 0 means the event is impossible and a probability of 1 means the event is sure to happen.

We can also define probability as the fraction of desired outcomes over the total number of outcomes. To show an example: Suppose we want to calculate the chance of getting 1 on a 6 sided die. We have 1 desired outcome (getting a 1) and 6 possible outcomes (please note that the outcomes are *mutually exclusive*: you cannot get both a 1 and a 6 on a single die, and you cannot have more than one event happen at the same time if events are mutually exclusive). Thus, the probability of getting a 1 on a 6 sided die is 1/6.

## Probability of Union of Events
In set theory or logic, the union ($\cup$) stands for "or" (I'm oversimplifying but let's use this definition first). Let's say that we are still rolling the same 6 sided die, however this time we want to see the chances of getting a 1 or 6. Because we are rolling only one die, we do not have to worry about calculating the chances of getting a 1 AND 6. \
Thus, we have two desired outcomes: getting a 1, and getting a 6. There are still 6 total outcomes, so the probability is 1/3. You may have also noticed that this is the same as simply adding the probabilities of getting a 1 and getting a 6. This applies to all mutually exclusive events, you can simply add their probabilities.

## Probability of Intersection of Events
Now let's say I want to roll 2 six sided dice. If i were to try and find the probability that i get 1 on the first die and 6 on the second, then I would have 1 desired outcome and 36 total outcomes (there are 6 sides on the first die, for each number on the first die, there is are 6 possible numbers for the second die). This is the intersection ($\cap$) of two events, in other words, when two events happen in the same time. Usually, the probabilities of events are multiplied together. \
To better understand why probabilities are multiplied together, remember that the probability is just the fraction of desired outcomes over the total outcomes. We multiply desired outcomes together: There is 1 way of getting a 1, and for each way of getting a 1 we have 1 way of getting a 6. Or for a better example: choosing two colors from Red, Green, and Blue (we can repeat colors). There are 3 ways of choosing the first color. Now we have chosen the first color, we have 3 choices for the second color. Since we have 3 ways of choosing the first color and 3 choices of choosing a second color for each choice of first color, then we have $3 \times 3 = 9$ ways of choosing two colors. \
For the total probability, we simply multiply the total probabilities of both events following from our argument above. There are 6 possible numbers on the first die, and for each number of a die, there are 6 possible numbers on the second die. Therefore, there are 36 possible total outcomes.