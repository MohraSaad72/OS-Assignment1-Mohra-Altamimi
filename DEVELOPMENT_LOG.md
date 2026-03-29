# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [March 27, 2026, 3:00 PM]
**What I did**: Set up the project and understood the base code

**Details**: 
-Opened the assignment project and reviewed the provided code
-Understood how threads and processes are structured
-Ran the program for the first time to see the initial output

**Challenges**: Understanding how the ready queue and thread mapping work together

**Solution**: Carefully read the code and traced execution step by step
**Time spent**: 1.5 hours

---

## Your Development Log:

### Entry 2 - [March 28, 2026, 5:30 PM]
**What I did**: Reviewed the code and planned implementation

**Details**: Revisited the project structure and understood how scheduling is handled
Analyzed how threads are executed step by step
Planned how to implement Round-Robin logic and additional features

**Challenges**: Understanding how all components (threads, queue, and process data) interact together

**Solution**: Spent time reading the code carefully and writing down the execution flow before coding

**Time spent**: 1 hour

---

### Entry 3 - [March 29, 2026, 2:00 PM]
**What I did**: Implemented Feature 1

**Details**: Added priority as an attribute to each process
Updated process initialization to include priority values
Modified output to display process priority

**Challenges**: Understanding how to integrate priority without affecting scheduling logic

**Solution**: Kept Round-Robin logic unchanged and only added priority as additional information

**Time spent**: 1 hour

---

### Entry 4 - [March 29, 2026, 6:00 PM]
**What I did**: Implemented Feature 2

**Details**: Added a counter to track the number of context switches
Incremented the counter after each quantum execution
Displayed the total context switches in the output

**Challenges**: Finding the correct place to increment the context switch counter

**Solution**: Placed the counter update right after each process yields the CPU

**Time spent**: 1.5 hours

---

### Entry 5 - [March 29, 2026, 9:30 PM]
**What I did**: Implemented Feature 3

**Details**:Used processMap to access process data correctly
Calculated waiting time based on execution order
Added summary section showing waiting time results 

**Challenges**:Errors due to accessing private variables and incorrect calculations 

**Solution**: Used getter methods and validated results through testing

**Time spent**: 2 hours

---



### Entry 6 - [Optional - Date and Time]
**What I did**: 

**Details**: 

**Challenges**: 

**Solution**: 

**Time spent**: 

---

## Summary

**Total time spent on assignment**: 7 hours

**Most challenging part**: Implementing the waiting time calculation and correctly mapping each thread to its corresponding process using processMap

**Most interesting learning**: Knowing how threads mimic CPU execution and how Round-Robin scheduling operates in reality

**What I would do differently next time**: Start earlier and break down the implementation into smaller planned steps
