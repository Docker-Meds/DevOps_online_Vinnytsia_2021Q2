## TASK1

1. Configured static ip addresses on virtual machines
> - VM1 = 10.20.20.18/24 (enp0s3 internal) and 10.0.3.15/24 (enp0s8 NAT)
> - VN2 = 10.20.20.20/24 (enp0s3 internal) 
2. Enable ip_forwarding on VM1 : echo 1 > /proc/sys/net/ipv4/ip_forward
3. Configured  iptables to enable masquerading on VM1
> /sbin/iptables -t nat -A POSTROUTING -o enp0s8 -j MASQUERADE   
> /sbin/iptables -A FORWARD -i enp0s8 -o enp0s3 -m state --state RELATED,ESTABLISHED -j ACCEPT   
> /sbin/iptables -A FORWARD -i enp0s3 -o enp0s8 -j ACCEP   
4. traceroute google.com.ua

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.1/images/2.PNG)   

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.1/images/3.PNG)  
