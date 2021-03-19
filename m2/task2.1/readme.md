## My work list

### PART 1. HYPERVISORS
* Hyper-V, vSphere Hypervisor, KVM(XEN)
* Hyper-v doesn't support usb devices, vSphere speed  is almost without loss of power of the guest machine, KVM uses hardware capabilities in virtualization

### PART 2. WORK WITH VIRTUALBOX
1. Downloaded and installed VirtualBox
2. Enabled virtualization in bios
3. Downloaded Ubuntu Server 18.04LTS and created VM1_yevhen_ladikov machine
4. I cloned VM1_yevhen_ladikov machine and called it VM2_yevhen_ladikov machine
5. Created group "Test Group" of two virtual machine, added machine and detached it
6. For VM1_yevhen_ladikov made snapshots 
7. Stopped VM2_yevhen_ladikov and exported VM2_Yevhen_Ladiukov.ova file
8. Imported Virtual machine and renamed it on VM3_Yevhen_Ladiukov
9. Connected the USB-flash drive and mount ports of the host machine to the VM1_Yevhen_Ladiukov
10. Created SMB folder and shared , changed virtual network settings 
11. Configured Port Forwarding rule with NAT
12. Used CLI VBoxManage modify vm

![Image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m2/task2.1/images/image_2021-03-18_12-11-09.png)

### PART 3. WORK WITH VAGRANT
1. Vagrant has already been installed on my workstation
2. Created folder "ladiukov"  and went to the folder
3. Vagrant initialize hashicorp/precise64 and startup VM
4. Connected to the VM by ssh port 2222 , it is time zone UTC 0 on a virtual machin
5. Created ubuntu/trusty64 and installed nginx
6. Changed port in vagrandfile and reloaded
7. nginx work on 8080 port

![Image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m2/task2.1/images/image_2021-03-18_14-42-05.png)

![Image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m2/task2.1/images/image_2021-03-18_15-50-57.png)
