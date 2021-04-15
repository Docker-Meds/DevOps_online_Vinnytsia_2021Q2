## TASK5.3

### PART1

1. Described status 
> 1. RUNNING & RUNNABLE
> 2. INTERRRUPTABLE_SLEEP
> 3. UNINTERRUPTABLE_SLEEP
> 4. STOPPED
> 4. ZOMBIE
2. Used command pstree : pstree -a, pstree -h, pstree -H PID
3./proc is very special in that it is also a virtual filesystem. It's sometimes referred to as a process information pseudo-file system, used like top, ps, w
4. Used command /proc/cpuinfo, lscpu, lshw  
5. Used command ps : ps aux, ps auxf, ps -ef, ps -f -U USERNAME
6. Kernel processed sudo ps --ppid=2 --pid=2, users sudo ps -N --ppid=2 --pid=2
7. Describe statuses of processed
> - PID 	The process ID of each task 
> - User 	The username of task owner
> - PR 	Priority Can be 20(highest) or -20(lowest)
> - NI 	The nice value of a task 
> - VIRT 	Virtual memory used (kb)
> - RES 	Physical memory used (kb)
> - SHR 	Shared memory used (kb)
