# Handy-OS
This an app which calculates fault occured in main memory by using page replacement algorithms.


Things to know for understanding this APP

Ø A basic idea on page replacement algorithms which we were taught in class and implemented in the lab, we were capable of coding all     page replacement algorithms in java.

Ø A very basic knowledge of Database which is linked with the java code in android studio.
  Adding interface with android studio.



Knowledge on our topics:

Page Fault:
             A page fault is a type of exception raised by computer hardware when a running program accesses a memory page that is not currently mapped by the memory management unit into the virtual address space of a process.


Page Replacement Algorithms:
                        Page replacement algorithms decide which memory pages to page out, sometimes called swap out, or write to disk, when a page of memory needs to be allocated. Page replacement happens when a requested page is not in memory (page fault) and a free page cannot be used to satisfy the allocation, either because there are none.


Types of page replacement algorithms used:


1. First in First Out: 
                   This is the simplest page replacement algorithm. In this algorithm, operating system keeps track of all pages in the memory in a queue, oldest page is in the front of the queue. When a page needs to be replaced page in the front of the queue is selected for removal. While FIFO is cheap and intuitive, it performs poorly in practical application. Thus, it is rarely used. This algorithm experiences Belady's anomaly.


2. Least Recently Used: 
                   In this algorithm page will be replaced which is least recently used. LRU works on the idea that pages that have been most heavily used in the past few instructions are most likely to be used heavily in the next few instructions too. While LRU can provide near-optimal performance in theory, it is rather expensive to implement in practice. The difficulty is that the list must be updated on every memory reference. Finding a page in the list, deleting it, and then moving it to the front is a very time consuming operation, even in hardware.
                   
                   
3. Optimal Replacement Algorithm:
                              In this algorithm, OS replaces the page that will not be used for the longest period of time in future. If one page will not be used for 8 million instructions and another page will not be used for 6 million instructions, removing the former pushes the page fault that will fetch it back as far into the future as possible. The only problem with this algorithm is that it is unrealizable. At the time of the page fault, the operating system has no way of knowing when each of the pages will be referenced next.
