Your Dice is Not Fair
=====================

Everyone who went to high school (at least nowsadays) should have some access to the theory of probability, the "study of coins and dice and whatsnot".

I would like to point out a misconception about the theory of probability and how things actually work in reality.

OK. Let us start with a dice. In rudimentary probability theory, one is taught that the probability a.k.a. the likelihood of landing on any face, say 1, is 1/6, either via

 * The intuitive formula: Probability = Number of desired outcomes divided by the number of all possible outcomes.
   In this case, there is only one desired outcomes (landing a 1 face) and there are six possible outcomes.

 * A more robust theory: We have to introduce the concepts of
    - The **set of outcomes** X, in case of rolling a typical dice X = {1, 2, ..., 6}
    - An **event** is a subset of X, for example, {1}, {2, 5}, ... (When X is infinite, there needs to be some restriction on the kind of subsets allowed.)
    - A **probability distribution** on X is a function P on the set of events satisfying certain intuitive conditions such as
       1. P(X) = 1, the total probability is 1. For example, if the dice has 6 faces, we are 100% certain to get one of the faces.
       2. P(A) + P(B) = P(A U B) if A and B are disjoint.
   With this more complicated machinery, we will see how the intuitive method fall short: A dice needs not be fair.
   There are probability distributions for the possible outcomes of a dice that are not 1/6 for each face.
   Furthermore, this yields another explanation for the probability of getting a 1: By rule 2, we have
      P({1}) + P({2}) + ... P({6}) = P({1,2,...,6})
   and by rule 1,
      P({1,2,...,6}) = 1.
   So
      P(1) + P(2) + ... P(6) = 1.
   Now, if the face is carefully manufactured to ensure balancing weight on all sides, **there is NO physical reason** that we have a higher chance of rolling one face over the other.
   In other words, we **expect** P(1) = P(2) = ... = P(6).
   This leads to P(1) = P(2) = ... = P(6) = 1/6 on account of the equation P(1) + P(2) + ... P(6) = 1.

All is right except **there is a physical reason** that we have a higher chance of rolling one face over the other.

 * Imagine yourself testing whether a dice manufactured by a company is actually fair. How would you do it?
 * You could roll a dice a _million_ times and count the frequencies where a certain face show up.
   If the frequencies are "close enough", then we can say the dice is fair.
 * Or you could be like me: Make a _robot_ to do it.
   (I definitely don't want to roll a dice a million times.)
 * Then you have a problem: Why do the robot keep rolling 1?

And you found out the issue:
 * A robot is different from a human being in that **it could REPLICATE the exact motion** for a million times (with very small error assuming good engineering).
 * In a closed environment (e.g. vacuum so that you can be sure that there is no external factor affecting the dice making it unfair), the dice follows the Newtonian physics.
 * So if the robot _performs the same physical motion_ to roll the dice, with its initial state unchanged (example, the face 1 is always up), the physics kicks in the same way and you are seeing the same outcome.
 * If you have access to a vacuum room, you can perform the experiment yourself: Say, you throw by simply dropping it from 10cm above the table top startig with its face 1 upward.
   Maybe use a metal dice with a side of 10cm.
   Are you expecting a different result in different time of rolling?
 * Would you be happy if someone rolls the dice by simply "putting it on the table" when playing table top games?

So the upshot is: In reality, **whether a dice is fair or not depends on you** (or how you throw it).
It is your unpredictable way of throwing the dice each time that gives its random nature.
