## GNU/LINUX ESSENTIAL

### TASK 1

1. Change password root user , sudo passwd root.
2. Used command "who -H -a -u, ps -u username".
3. Change user info, sudo usermod -c "Yevhen Ladiukov" username.
4. Used command "man -f -k -w nano".
5. Used command less "less -N -X first.sh"
6. Created nano ~/.plan and added txt
7. Used command "ls , -l, -ll, -la"

### TASK 2
1. Used command "tree, -a, -f, -d, -df, -f -L 2, tree -f -P a*, tree -f -L 2 -P c*
2. Used commnad "file, file -i *.txt, file -b *.bin 
3. Used command "cd, cd ~, cd .., cd ../, cd ../..
4. Described command ls, -l it's long format, -a it's all format(and hide)
5. Used command mkdir, touch, cd, cat or less, rm -r -f
6. Created dir test and export .bash_history "export HISTFILE=/home/$USER/.bash_history"
> - mv file .bash_history to labwork2
> - created soft link "ln -s test/labwork2 labwork2"
> - created hard link "ln test/labwork2 labwork2.1" it's duplicate file
> - changed file "echo hello > labwork2" hard and soft link changed file
> - rename hard and soft link
> - deleted labwork2
> - soft doesn't work, hard work because it's dublikate file
7. Installed mlocate and finded traceroute, squid.
8. Used command lsblk and df -h, -a, -l, -P, --help.
9. Used cammand wc, wc .bash_history, -w, -l .
10. Used cammand find, sudo find /etc -name "host*" .
11. Used command grep,  grep ss /etc/* , grep ss /etc/* | wc .
12. Used command cat,  cat /etc/* > catfile.txt or ls /etc > lsfile.txt
13. Device types looked at devices ls -l /dev , sda - hard disk
> - Listing USB Devices  "lsusb"
> - Listing PCI Devices  "lspci" 
> - Listing SCSI Devices "lsscsi"
14. Determined to type file system df -Th or lsbdk -f, tmpfs -temp files, squashfs -compressed read-only file system
15. 5 most-recently modified files in /etc , used command ls /etc -1t | tail -5
> - deluser.conf
> - screenrc
> - fuse.conf
> - protocols
> - rpc

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-08_09-40-42.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-08_10-20-39.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-08_11-32-34.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-08_12-06-59.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_09-59-04.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_10-54-02.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_11-34-35.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_12-53-08.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_13-26-17.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_13-31-15.png)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m5/task5.1/images/image_2021-04-09_15-16-04.png)

