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

## Cleaning up

To clean up all binary files, you must use the command: make clean. Make sure that you're in the root directory, i.e. the same directory as the makefile.
