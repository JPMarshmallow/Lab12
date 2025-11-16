# Lab 11 - Counters and Dividers

In this lab, we learned how to make clock dividers from two types of counters.


## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Questions
* We learned how to create a modulo counter using full adders and d-flipflops.
* We learned how to create a ripped counter using t-flipflops.
* We learned how to create a threshold for our counters to know when to restart counting.

### 1 - Why does the Modulo Counter actually divide clocks by 2 * Count?
* The modulo counter divides the clocks by the modulus N. It goes thru N number of states before restarting at 0.
* It uses the adder circuits which take 2 cycles from the previous latch for each cycle it has.

### 2 - Why does the ring counter's output go to all 1s on the first clock cycle?
* Because the Q output of the last d-flipflop, is also used as an input. This configuration creates what can be considered a "down counter" which starts from the highest value and counts down.

### 3 - What width of ring counter would you use to get to an output of ~1KHz?
* log2(1000) = 9.97. Therefore a width of 10 is required.
