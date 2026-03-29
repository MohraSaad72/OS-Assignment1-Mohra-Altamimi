# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:A process is a stand-alone program that is running and has its own memory and system resources. A thread, on the other hand, is a small unit of execution that shares memory with other threads inside a process. Compared to processes, threads require less overhead during creation and context switching. In this project, a Round-Robin scheduling mechanism was employed to mimic many processes utilizing threads. Data structures like the ready queue can be shared and executed efficiently with this method. Because of their performance and reduced resource use, threads are therefore better suited for this simulation.**

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:A process in Round-Robin scheduling gets moved to the end of the ready queue and waits for its next turn if it does not complete within its time quantum. The software output makes this behavior quite evident. Process P1, for instance, begins execution with a burst time of 5229 ms and runs for a single quantum of 4000 ms. It then concedes the CPU and is re-added to the ready queue because it still has 1229 milliseconds left.**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:
P1 executing quantum [4000ms] 
P1 completed quantum 4000ms
Remaining time: 1229ms 
P1 yields CPU for context switch 
 P1 added to ready queue

**Explanation of example:**
This illustration demonstrates that P1 failed to finish execution within the allotted time period. Consequently, P1 is positioned at the end of the ready queue and a context transition takes place. It won't get another turn until every other process in the queue has finished. Later in the output, P1 runs once again for 1229 milliseconds until finishing, illustrating how Round-Robin scheduling iterates across processes until they are finished.



## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

. **New**:
   P1 is in the New state when it is first created and added to the ready queue, as shown in the output:
   P1 added to ready queue (Priority: 4) │ Burst time: 5229ms


2. **Runnable**:
   P1 enters the Runnable state after being added to the ready queue and waiting for its turn in the scheduling cycle, as shown in the queue:

[P2 → P3 → ... → P14]

3. **Running**:
   P1 moves to the Running state when it starts executing its time quantum:


▶ P1 executing quantum [4000ms]


4. **Waiting**:
   After completing its time quantum, P1 enters a waiting state while other processes execute. This is observed when it yields the CPU and is re-added to the queue:


↻ P1 yields CPU for context switch
➕ P1 added to ready queue


5. **Terminated**:
   P1 reaches the Terminated state after finishing all its remaining execution time:


▶ P1 executing quantum [1229ms]
Remaining time: 0ms
✓ P1 finished execution!


This sequence shows the full lifecycle of P1 from creation to completion based on the actual program output.



## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: Web Server Handling Multiple Requests

**Description**: 
Multiple client requests, including loading webpages or responding to API calls, are processed concurrently by a web server.

**Why Round-Robin works well here**: 
Every request is given an equal amount of CPU time thanks to round-robin scheduling. This enhances overall responsiveness by preventing any one request from obstructing others. Additionally, it offers balanced and predictable performance when managing a large number of users.

### Example 2: Operating System Task Scheduling

**Description**: 
Multiple programs, including background processes and user applications, are managed concurrently by an operating system.

**Why Round-Robin works well here**: 
The CPU can transition between processes using a set time quantum thanks to Round-Robin. This keeps people from starving and guarantees justice. In time-sharing systems, context switching is crucial since it enables all processes to advance.
---

## Summary

**Key concepts I understood through these questions:**
1. The distinction between processes and threads
2. The behavior of the ready queue and round-robin scheduling
3. State transitions and the thread lifetime


**Concepts I need to study more:**
1. Race situations and thread synchronization

2. Deadlocks and sophisticated concurrency ideas
