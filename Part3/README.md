# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to a repository to complete the task. Remember to also submit your answers to Blackboard

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > *Concurrency are techniques that make programs more usable and are used mostly on single processing units, but it may benefit from multiple processing units in regards to speed. Parallelism are techniques to make programs faster by performing several computations at the same time.
 The difference is concurrency is when two tasks can start, run, and complete in overlapping time periods, meanwhile parallelism is when tasks run at the same time, like on a multi-core processor.*
 
 ### Why have machines become increasingly multicore in the past decade?
 > *The reason for the increase in multicore on machines in the past decade, are that multicore contains multiple single cores. By having multiple, is it possible to handle more than one thread simultaneously.*
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > *Concurrency helps so that multiple processes that are assigned to different cores on a machine by the kernel, will all cores execute the process instructions at the same time.*
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Your answer here*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > *Your answer here*
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *Your answer here*
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *Your answer here*
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Your answer here*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *Your answer here*
