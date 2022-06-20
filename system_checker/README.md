#### Make a utility which check your system info about (CPU,Memomry, disk space etc ) 

- send a critical alert notification to slack if it crosses the threshold value (threshold value > 75%). 
- If the usage crosses the above 50% then it should only send a waring message 
- it should generate logs in the file /var/log/check_system.logs

```
./check_system.sh 
CPU 82% (75%)
MEM 72% (75%)
Disk space 46% (70%)
CRITICAL: CPU usage 82% which is above threshold sending alert to slack. 
WARNING: CPU usage above 50%.
```
Log format should look like this 

```
[Fri Jun 16 01:46:23 2022] [WARNING] [MEM: 72%]  
[Fri Jun 16 01:46:23 2022] [CRITICAL] [CPU: 82%]
[Fri Jun 16 01:46:23 2022] [NORMAL] [DISK SPACE: 42%]
```