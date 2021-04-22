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

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/4.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/7.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/6.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/8.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/9.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m6/task6.2/images/10.PNG)
