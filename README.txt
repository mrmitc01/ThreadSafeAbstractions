ThreadSafeAbstractions

The goal of this project is to implement a thread-safe, unbounded priority queue and to build a thread pool using the priority queue implementation.

The purposes of each of the following files are stated below:


pq.h - This declares the interface to the priority queue abstraction, namely, the type pq_t and the three functions pq_create(), pq_insert(), and pq_next().

threadpool.h - This declares the interface to the thread pool abstraction, namely, the type threadpool_t and the two functions tp_create() and tp_submit().

pqimpl.c - This will implement the three functions pq_create(), pq_insert(), and pq_next() for a priority queue.

threadpool.c - This will implement the thread pool abstraction, namely, the two functions tp_create() and tp_submit().

seqdriver.c -  This is a simple unit test program to verify that the implementation maintains priorities correctly.

pooldriver.c - This is a simple unit test program that creates a thread pool and submits tasks to it. Command-line parameters control the size of the pool and the number of tasks to submit. The tasks are defined in the driver program; each one simply prints its priority and a sequence number (indicating the order it was submitted to the pool), sleeps for a random number of seconds, and then prints a message indicating completion.

makefile - This will compile both the seqdriver and pooldriver programs.


Compile the source code by typing the following at the prompt $:
$ make

Code is available upon request
