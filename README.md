# DiskScheduling

# fcfs
First come first serve (FCFS) scheduling algorithm simply schedules the jobs according to their arrival time. The job which comes first in the ready queue will get the CPU first. The lesser the arrival time of the job, the sooner will the job get the CPU. FCFS scheduling may cause the problem of starvation if the burst time of the first process is the longest among all the jobs.

## Advantages of FCFS
Simple
Easy
First come, First serv
## Disadvantages of FCFS
The scheduling method is non preemptive, the process will run to the completion.
Due to the non-preemptive nature of the algorithm, the problem of starvation may occur.
Although it is easy to implement, but it is poor in performance since the average waiting time is higher as compare to other scheduling algorithms.
