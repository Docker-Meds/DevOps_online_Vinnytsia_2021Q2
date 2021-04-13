## LINUX ESSENTIAL

1. Added new user "teststudent" , used key  -u -g and -m.
2. Used cat /etc/passwd 
<p>(1)teststudent:(2)x:(3)1001:(4)1001:(5)Student:(6)/home/teststudent:(7)/bin/sh</p>
<p>1. Username
2. Password: stored in /etc/shadow file
3. User ID (UID)
4. Group ID (GID)
5. User ID Info
6. Home directory
7. Command/shell</p>


3. Used cat /etc/group
<p>(1)mysql:(2)x:(3)118:(4)teststudent</p>
<p>1.group_name 2.Password: Generally password is not used 3.Group ID (GID) 4.Group List</p>  


4. UID User ID: Each user must be assigned a user ID (UID). UID 0 (zero) is reserved for root and UIDs 1-99 are reserved for other predefined accounts. Further UID 100-999 are reserved by system for administrative and system accounts/groups.  
5. GID Group ID : is a text file which defines the groups to which users belong under Linux and UNIX operating system. Under Unix / Linux multiple users can be categorized into groups.  
6. Determine the user belonging to groups    groups [username]
7. Used command adduser and useradd "sudo useradd -m -G mysql,cdrom -s /bin/bash teststudent"
8. Used command usermod "sudo usermod -l student teststudent" or "usermod -u 1001 student" and change home directory "sudo usermod -d /home/newHomeDir -m student"  
9. Dir_skel is used to initiate home directory when a user is first created, "ls -lart /etc/skel"
10. Deleted users and mail spool : "sudo userdel -r student"
11. Locked and unlocked users : "usermod -L(lock) -U(unlock) student2"  or "passwd -l -u student2"
12. Changed password : "passwd --expire student2" or "chage -d 0 student"  
13. Used command ls : ls -l
<p>(1)drwxrwxr-x (2)3 (3)student (4)student  (5)4096 (6)Mar 11 13:11 (7)docker</p> 
<p>1.content permissions 2.number of links to the content 3.owner of the content 4.group owner of the content 5.size 6.last modified date / time of the content 7.file or directory name</p>  


14. Access rights: r-read w-write x-execute , ownership of linux files: users, groups. other. 
15. Used command chmod, chown, chgrp.
16. Used command umask, changed ~/.bashrc .
> - Files:644. The owner can read and modify the files. Group and others can only read the files  
> - Directories:755.The owner can cd into the directory, and list, read, modify, create or delete the files in the directory. Group and others can cd into the directory and list and read the files  
17. Used sticky bit, "sudo chmod o+t(1777) mydir"
18. Used command lsattr: 

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.2/images/image_2021-04-13_09-36-25.png)  
![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.2/images/image_2021-04-13_11-01-23.png)  
![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.2/images/image_2021-04-13_11-10-16.png)  
![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.2/images/image_2021-04-13_12-41-21.png)  
![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.2/images/image_2021-04-13_12-48-32.png)  
![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.2/images/image_2021-04-13_14-02-46.png)  
