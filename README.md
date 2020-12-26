# Random-Walk-Game-Logic
We plan to create a Dice game logic which will decide the odds of reaching Step number 60 of the Empire State Building in 100 rolls of the Dice. We would then simulate this sequence multiple times to calculate the probability of reaching step 60 in 100 tries using the Dice game logic.

Some pointers that might help with the code:
a. We have used a function random.seed() and set its value at 123. You can have a different value set as well in your code. What this does is to give out a sense of pseudo randomness in the results. Something like a consistent value of randomness.
b. To represent clumsiness of falling down we have used random number call between 0 and 1 and if it throws up .001 we set the steps value to Zero as is the rule.
c. We have used the function max(0,step-1) while decrementing by 1 as is the rule, so that any negative value don't creep up after decrementing.
d. We have created a numpy 2d array of the results to make it easy in interpreting and transposed it to give a good depiction while plotting it.
e. At the end we have used a for loop again to iterate through the results and check the number of times the last step value represented by ends is greater than 60.
