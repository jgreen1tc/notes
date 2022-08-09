Multiple CPUs can execute programs simultaneously

Tightly coupled multiprocessing - within a CEC, when a single CPU shares main memory with another CPU, all of them are controlled by a single Operating System (such as z/OS)

Loosely coupled multiprocessing - when a single CPU shares a common workload with others, but does not shre real storage and runs its own copy of z/OS
	ex - LPAR facility to run multiple z/OS images on one CEC or in a Parallel SysPlex environment