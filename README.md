# Introduction
Operating system (OS) is a collection or package of numerous soft-wares which act as an intermediary between the computer hardware and end user. It provides a means for the user to work with the computer. Operating system performs major functions like memory management, process scheduling and resource management. The need for a scheduling algorithm arises from the requirement for most modern systems to perform multitasking (execute more than one process at a time) and multiplexing (transmit multiple flows simultaneously). CPU Scheduling is the basis of multi programmed operating systems. By switching the CPU among the processes, the operating system can make the computer system productive.

# CPU Scheduler 
Whenever the CPU becomes idle, the operating system must select one of the processes in the ready queue to be executed. The selection process is carried out by the short-term scheduler or CPU Scheduler. The scheduler selects a process from the processes in memory that are ready to execute and allocate the CPU to that process.

# CPU SCHEDULING POLICIES
Generally, the policies of scheduling either pre-emptive or non-preemptive

# Non-preemptive scheduling
Non-preemptive occurs in a multiprogramming system which means the short-term scheduler permits the process to run until it terminates or in some cases waiting for an event.
In another word, the current process frees the CPU either by finishing or by changing to the state of waiting.

# Preemptive scheduling
Preemptive rules push the process which is active currently for releasing the CPU on particular events for instance, a clock interrupts, input & output interrupts and a call of the system. The process that is executed currently needs to release the CPU involuntarily if a high-priority process puts into the ready queue.

# CPU SCHEDULING ALGORITHMS
Scheduling stands for deciding which jobs run whenever there are more than runnable jobs. There are various objectives for competing these scheduling algorithms. These objectives are the throughput and turnaround time as well as the response time. In another term of meaning the scheduling of CPU is the procedure of identifying which process in the queue will allocate firstly to the CPU. Many types of well-known scheduling algorithms will be described in the next subsections.

# Priority scheduling for preemptive and non-preemptive types
In the priority scheduling algorithm, there is a classification of processes according to some system criteria depending on the processed type. The priority of the process is made by a group of measures and any process inserting the ready queue provides its importance as a priority. Only the priority number determines the allocating decision to the CPU for a process in a way that the high-value priority of the process will arrive at the CPU first or next. Two types of versions exist for this algorithm which is preemptive and non-preemptive. In the preemptive Type of this algorithm, the lowest priority process may be suffering from starvation in case of a process with big priority keep to coming to the ready queue.

# Characteristics of Priority Scheduling
* A CPU algorithm that schedules processes based on priority.
* It used in Operating systems for performing batch processes.
* If two jobs having the same priority are READY, it works on a FIRST COME, FIRST SERVED basis.
* In priority scheduling, a number is assigned to each process that indicates its priority level.
* Lower the number, higher is the priority.
* In this type of scheduling algorithm, if a newer process arrives, that is having a higher priority than the currently running process, then the currently running process is preempted.

# Advantages of priority scheduling
* Easy to use scheduling method
* Processes are executed on the basis of priority so high priority does not need to wait for long which saves time
* This method provides a good mechanism where the relative important of each process may be precisely defined.
* Suitable for applications with fluctuating time and resource requirements.

# Disadvantages of priority scheduling
* If the system eventually crashes, all low priority processes get lost.
* If high priority processes take lots of CPU time, then the lower priority processes may starve and will be postponed for an indefinite time.
* This scheduling algorithm may leave some low priority processes waiting indefinitely.
* A process will be blocked when it is ready to run but has to wait for the CPU because some other process is running currently.
* If a new higher priority process keeps on coming in the ready queue, then the process which is in the waiting state may need to wait for a long duration of time.

# Implementation:
1. First, we will input the processes with their burst time and priority. (𝑃𝑛 arrives earlier than 𝑃𝑛+1)
2. First process will schedule, which have the lowest arrival time, if two or more processes will have lowest arrival time, then whoever has higher priority will schedule first.
3. Now further processes will be schedule according to the arrival time and priority of the process.
4. Once all the processes have been arrived, we can schedule them based on their priority.

