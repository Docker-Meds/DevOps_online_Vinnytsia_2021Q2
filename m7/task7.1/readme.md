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
1.Search for ip that has most of requests  
#!/bin/bash  
file_out=out_script2  
awk '{ print $1}' $1 | sort | uniq -c | sort -nr | head -n1 > $file_out  
{  
read line1  
}<$file_out  
echo $line1  

2.search for that has most of requested page
#!/bin/bash  
file_out=out_script2  
awk '{ print $1}' $1 | sort | uniq -c | sort -nr | head -n1 > $file_out  
{  
read line1  
}<$file_out  
echo $line1  
