 ### Aim: Write a C program to implement the various process scheduling mechanisms such as Round Robin Scheduling.
 
## Algorithm
1: Start the process
2: Accept the number of processes in the ready Queue and time quantum (or) time slice
3: For each process in the ready Q, assign the process id and accept the CPU burst time
4: Calculate the no. of time slices for each process where
     No. of time slice for process(n) = burst time process(n)/time slice
5: If the burst time is less than the time slice then the no. of time slices =1.
6: Consider the ready queue is a circular Q, calculate
        (a) Waiting time for process(n) = waiting time of process(n-1)+ burst time of process(n-1 ) +
              the time difference in getting the CPU from process(n-1)
        (b) Turn around time for process(n) = waiting time of process(n) + burst time of process(n)+ the
               time difference in getting CPU from process(n).
7: Calculate
       (a) Average waiting time = Total waiting Time / Number of process
    (b) Average Turnaround time = Total Turnaround Time / Number of process Step 
8: Stop the proces.
