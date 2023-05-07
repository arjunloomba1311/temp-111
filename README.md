## UID: 605809574

## You Spin Me Round Robin

This is an implementation of Round Robin Scheduler for a given workload and quantum length.

## Building

Open the terminal with a bash session. Navigate to the root directory of the folder. Call Make to compile the c files, and generate the executable. This is enabled through the makefile

```
make
```

## Running

After generating the executable you may run the Round Robin Simulation script by passing in two arguments. The first is a text file containing the process serial number, arrival time, burst time, and the total number of processes. The second is the quantum length or time slice. Here's an example on how the code is run:

```
./rr processes.txt 3
```

Let's give an example on running the script. Here's a sample text file: 

```
4
1, 0, 7
2, 2, 4
3, 4, 1
4, 5, 4

```

The solitary number on the first row represents the number of processes, the first column in the serial number for processes, the second column is the process arrival time, and the third is the burst time.

Output is retrieved in terms of the average waiting time and the average response time for the processes.

```
.\rr processes.txt 3
```

Output is 

```
Average waiting time: 7.00
Average response time: 2.75
```

## Cleaning up

To clean up all binary files, you must use the command: make clean. Make sure that you're in the root directory, i.e. the same directory as the makefile.

```
make clean
```
