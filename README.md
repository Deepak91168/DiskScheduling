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

# clook
Circular-LOOK Algorithm is an improved version of the LOOK Algorithm.
Head starts from the first request at one end of the disk and moves towards the last request at the other end servicing all the requests in between.
After reaching the last request at the other end, head reverses its direction.
It then returns to the first request at the starting end without servicing any request in between.
The same process repeats.

# Look
LOOK is the advanced version of SCAN (elevator) disk scheduling algorithm which gives slightly better seek time than any other algorithm in the hierarchy (FCFS->SRTF->SCAN->C-SCAN->LOOK). The LOOK algorithm services request similarly as SCAN algorithm meanwhile it also “looks” ahead as if there are more tracks that are needed to be serviced in the same direction. If there are no pending requests in the moving direction the head reverses the direction and start servicing requests in the opposite direction.
The main reason behind the better performance of LOOK algorithm in comparison to SCAN is because in this algorithm the head is not allowed to move till the end of the disk.

# cscan
The circular SCAN (C-SCAN) scheduling algorithm is a modified version of the SCAN disk scheduling algorithm that deals with the inefficiency of the SCAN algorithm by servicing the requests more uniformly. Like SCAN (Elevator Algorithm) C-SCAN moves the head from one end servicing all the requests to the other end. However, as soon as the head reaches the other end, it immediately returns to the beginning of the disk without servicing any requests on the return trip (see chart below) and starts servicing again once reaches the beginning. This is also known as the “Circular Elevator Algorithm” as it essentially treats the cylinders as a circular list that wraps around from the final cylinder to the first one.

## Advantages of C-SCAN (Circular Elevator) Disk Scheduling Algorithm:
Works well with moderate to heavy loads.
It provides better response time and uniform waiting time.
## Disadvantages of C-SCAN (Circular Elevator) Disk Scheduling Algorithm:
May not be fair to service requests for tracks at the extreme end.
It has more seek movements as compared to the SCAN Algorithm.
