## Linux administration with bash

### A

#!/bin/bash  

man bash | grep "(.-.*)$" -A1  

echo "What do yo want to scan: subnet(--all)/port (--target)"  
read use  
echo subnet  

if [[ "$use" == "--all" ]]; then  
 nmap -sn 10.10.10.1/24  
fi  

echo "What do yo want to scan: subnet(--all)/port (--target)"  
read use  
echo ports  
if [[ "$use" == "--target" ]]; then  
sudo nmap -PE localhost  
fi  

### B
#### 1.Search for ip that has most of requests  
#!/bin/bash  
file_out=out_script2  
awk '{ print $1}' $1 | sort | uniq -c | sort -nr > $file_out  
{  
read line1  
}<$file_out  
echo $line1  

#### 2.Search the most requested pages
#!/bin/bash  
file_out=out_script7  
awk -F\" '{print $4,$5}' $1 | sort | uniq -c | sort -fr  
echo END  

#### 3.Search how many requests were there from each ip  
#!/bin/bash  
file_out=out_script3  
awk '{ print $1}' $1 | sort | uniq -c | sort -nr | head -n20  
echo $1  

#### 4.Search page with status 404 
#!/bin/bash  
file_out=out_script7  
awk '{ if($9 == 404) { print $7 } }' $1 | sort | uniq -c | sort -fr  
echo END  

#### 5.Search what time did site get the most requests  
#!/bin/bash  
file_out=out_script6  
awk '{print $1,$4,$5}' apache_logs.txt | sort | uniq -c | sort -fr | head -n 30  
echo END  

#### 6.Search what search bots have accessed the site  
#!/bin/bash  
file_out=out_script7  
awk -F\" '{print $1 $6}' $1 | sort | uniq -c | sort -fr  
echo END  



![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/0.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/1.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/2.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/3.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/4.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/5.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/6.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/7.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/8.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m7/task7.1/images/9.PNG)
