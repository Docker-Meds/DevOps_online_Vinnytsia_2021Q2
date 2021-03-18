## My work list

### PART 1. HYPERVISORS
* Hyper-V, vSphere Hypervisor, KVM(XEN)
* Hyper-v doesn't support usb devices,vSphere speed of the guest machine is almost without loss of power, KVM uses hardware capabilities in virtualization

### PART 2. WORK WITH VIRTUALBOX
1. Download and install VirtualBox
2. Enable virtualization in bios
3. Download Ubuntu Server 18.04LTS and created VM1_yevhen_ladikov machine
4. I Cloned VM1_yevhen_ladikov machine by creating a VM1_yevhen_ladikov machine
5. Create group "Test Group" of two virtual machine, add machine and detach it
6. For VM1_yevhen_ladikov maked snapshots 
7. Stop VM2_yevhen_ladikov and export VM2_Yevhen_Ladiukov.ova file
8. Import Virtual machine and rename in VM3_Yevhen_Ladiukov
9. Connect the USB-flash drive and mount ports of the host machine to the VM1_Yevhen_Ladiukov
10. Create SMB folder and share , change virtual network setings 
11. Configuring Port Forwarding rule with NAT
12. Uses CLI VBoxManage modifyvm

### PART 3. WORK WITH VAGRANT
1. Vagrant has already been installed on my workstation
2. Create folder "ladiukov"  and go to the folder
3. Vagrant init hashicorp/precise64  and startup VM
4. Connect to the VM by ssh port 2222 , on a virtual machine time zone  UTC 0
5. Create ubuntu/trusty64 and install nginx
6. Change port in vagrandfile and reload
7. nginx work on 8080 port
