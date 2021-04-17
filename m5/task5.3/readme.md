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
6. Kernel processes sudo ps --ppid=2 --pid=2, users sudo ps -N --ppid=2 --pid=2
7. Describe statuses of processed
> - PID 	The process ID of each task 
> - User 	The username of task owner
> - PR 	Priority Can be 20(highest) or -20(lowest)
> - NI 	The nice value of a task 
> - VIRT 	Virtual memory used (kb)
> - RES 	Physical memory used (kb)
> - SHR 	Shared memory used (kb)
8. print user processes : top -u USERNAME or ps -u USERNAME
9. Used command : lsof, pidstat, top, htop, ps, netstat
10. Described colums top
> - PID: Shows task’s unique process id.
> - PR: Stands for priority of the task.
> - SHR: Represents the amount of shared memory used by a task.
> - VIRT: Total virtual memory used by the task.
> - USER: User name of owner of task.
> - %CPU: Represents the CPU usage.
> - TIME+: CPU Time, the same as ‘TIME’, but reflecting more granularity through hundredths of a second.
> - SHR: Represents the Shared Memory size (kb) used by a task.
> - NI: Represents a Nice Value of task.
> - %MEM: Shows the Memory usage of task
11. Interactive command TOP :
> - Enter or Space :Refresh
> - h : Help
> - k : kill task
> - q : Quit from top
> - M : Same as above but sorts by Memory usage
> - P : This command sorts all displayed processes by CPU usage
12. Sort processes : ps -p <pid>, ps -G <groupname>, ps -ef, ps -ef --sort user,pid
13. Used commands nice and renice: nice -n -5 mysql , renice -n -2  -u mysql
14. top command, press r.  PID  Give renice value (from -20 to +19)
15. Used command kill : kill -l , kill PID, kill -9
16. Used commands jobs, fg, bg, nohup
> - nohup: To run a process in no hangup status
> - jobs: Display a list of the jobs with their status
> - fg: Move a background job into the foreground
> - bg: Resume suspended jobs by running them as background jobs

### PART2

1. Worked with openSSH client in Windows OS : ssh.exe, scp.exe, ssh-keygen.exe
2. Improved to Secure Open SSH , nano /etc/ssh/sshd_config
> - Configure Idle Timeout Interval :ClientAliveInterval 360, ClientAliveCountMax 0
> - Disable Empty Passwords : PermitEmptyPasswords no
> - Disable Root Logins : PermitRootLogin no
> - Use another port SSH : 22 to changed 22200
> - Worked with SSh key : ssh-keygen -t rsa -b 4096, ssh-keygen -t rsa -b 4096 -o -a 250 -C “Student” , 
3. Setup port forwardiing  for ssh client for host to virtual machine behind NAT: 2222 -> 22
4. Used wireshark , intercept ssh traffic  while authorizing the remote client

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/8.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/11.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/12.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/14.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/1.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/2.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/3.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/4.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/4.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/5.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/6.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/7.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/9.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/10.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.3/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-15%2015-11-36.png)
