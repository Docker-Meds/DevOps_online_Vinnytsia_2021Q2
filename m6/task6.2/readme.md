## Configuring DHCP, DNS servers

1. Installed isc-dhcp-server on VM1.
2. Configured DHCP server VM1 = 10.20.20.18/24 (enp0s3 internal) range 10.20.20.10 - 30.
3. Enablde dhcp client on V2, VM3.
4. VN2 = 10.20.20.10,   VN2 = 10.20.20.11.
5. Installed bind9 on VM1 =10.20.20.18.
6. Configuration
> - Private network address is 10.20.20.0/24.
> - Private network name is hiepam.com.
> - IP address of DNS server for private network is 10.20.20.18. This DNS server uses recursive query.
7. Created dns zone "hiepam.com".
8. Add interface bridge on VM3 = 10.20.20.10/24 (enp0s3 internal dhcp4), 10.10.10.122/24 (enp0s8 bridge dhcp4)
9. Installed quagga on VM3.
10. Configure ospfd.conf.  
> interface enp0s3  
> router ospf  
> ospf router-id 192.168.1.1  
> network 10.20.20.1/24 area 0.0.0.0  
> network 10.10.10.0/24 area 0.0.0.0  
11. Checked traceroute google.com.ua and my private dns server server.hiepam.com .

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/4.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/7.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/6.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/8.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/9.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/10.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/13.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/14.PNG)  

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/15.PNG)  
