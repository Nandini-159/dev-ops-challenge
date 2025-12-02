Commands which will be used :
command: top
To check :
Processes consuming high CPU usage,
Any processes in zombie state

Command:
pidstat -u 1 5
to check : Specific PIDs constantly using high CPU

command : 
free -m
vmstat 1 5
to check :
Swap usage increasing

command : ps aux service
ps aux | grep mysql
to check :
 Check application-level issue,
 check long running db queries 



