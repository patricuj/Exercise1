# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to a repository to complete the task. Remember to also submit your answers to Blackboard

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency are techniques that make programs more usable and are used mostly on single processing units, but it may benefit from multiple processing units in regard to speed. Parallelism are techniques to make programs faster by performing several computations at the same time.
The difference is concurrency is that tasks can start, run, and complete in overlapping time periods, meanwhile parallelism is when tasks run at the same time, like on a multi-core processor. 
 
 ### Why have machines become increasingly multicore in the past decade?
 > The reason for the increase in multicore on machines in the past decade, are that multicore contains multiple single cores. By having multiple, is it possible to handle more than one thread simultaneously. 
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Concurrency helps so that multiple processes that are assigned to different cores on a machine by the kernel, will all cores execute the process instructions at the same time. 
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Creating concurrent programs can make a programmer's life easier, but it is harder to have order on things with concurrent programs. For most people I would say that creating concurrent programs make their lives harder, but if the programmer is a hard worker and has the knowledge concurrent programs will make their lives better. 
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > A process is a program combined with the state of all the threads executing in the program, meanwhile a thread executes a lot of commands in a line. Then you have green threading that is threads that are scheduled by a runtime library or virtual machine instead of natively by the underlying operating system (OS). Coroutines are in other words cooperative function. You have a A Function and a B Function, these will cooperate with each other where the A Function starts its functions then the B function will kick off where the A function stopped and it will continue like this until all functions are done
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > (C/POSIX) creates `pthread_create()` that is the coding for muktithreading.
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > It makes it so that threads can always executing one at the time even with multicore processes.
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > The workaround is the Python threading module, because it provides a very simple and intuitive API for spawning multiple threads.
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > The `func GOMAXPROCS(n int) int` sets the maximum number of CPUs that can be simultaneously executed and returns the previous setting.
