# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:This assignment taught me how multithreading enables several activities to run concurrently within a single program. I comprehended how Java threads are generated and run using join() and start(). I utilized threads to represent processes while working on the Round Robin simulation, and I saw how each thread received CPU time in turn. This made it easier for me to comprehend how scheduling functions in an actual system. Additionally, I saw that threads share memory, which speeds them up over processes but necessitates careful management. The way thread states change during execution—particularly when using sleep() to simulate time—was one crucial lesson I picked up. All things considered, this assignment enabled me to go beyond merely understanding multithreading in theory to actually using it in code.**

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:Implementing the waiting time functionality was the most difficult aspect of this task. When I first attempted to directly access variables inside the Process class that were designated as private, I encountered problems. Compilation problems resulted from this, making it challenging to determine the accurate waiting time. Understanding how to properly map each thread to its matching process using the processMap was another difficulty. Additionally, I had trouble locating the waiting time computation within the loop. The results would be erroneous if they were positioned wrongly. This section necessitated a better comprehension of thread execution and object-oriented programming. Although difficult, it improved my debugging abilities.**

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:I began by closely examining the error messages to determine the location of the issue in order to overcome these obstacles. I came to the conclusion that, rather than directly accessing private variables, I needed to use getter and setter methods. In order to accurately extract the process linked to each thread, I also went over the processMap's structure. I verified my logic step-by-step using debugging tools like printing intermediate values. I also went over the encapsulation and threading class materials and examples again. The problem was easier to address when it was divided into smaller components. I eventually managed to correct the mistakes and properly implement the feature.**

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:In practical applications, multithreading is frequently employed to enhance responsiveness and performance. For instance, web browsers allow users to navigate effectively by using many threads to load multiple tabs at once. I observed in my assignment how threads mimic the operation of operating systems by simulating several processes executing in a CPU. Another example is in video games, where different threads manage physics, graphics, and user input simultaneously. Threads are also used by mobile applications to carry out background operations without causing the user interface to freeze. This task made me realize how crucial multithreading is to building responsive and effective systems. It improved my comprehension of how these ideas are used in actual software development.**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?

I want to know more about preventing race situations and thread synchronization. Additionally, I'm curious about how deadlocks happen and how to avoid them. Beyond Round Robin, I also wish to investigate more sophisticated scheduling techniques.

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
