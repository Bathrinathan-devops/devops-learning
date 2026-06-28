## Day 11 - System Health Monitor Project

#!/bin/bash
#System Health Monitor
#Author : Bathrinathan
#Date : June 2026
echo "=========================================="
echo "           SYSTEM HEALTH MONITOR"         "
echo "=========================================="

check_memory() {
 echo "checking memory.."
 free -h
 echo :-----------------------------------------"
 }

 check_disk() {
   echo "Checking Disk Space..."
   df -h
   echo "---------------------------------------"
   }

  check_processes() {
  echo "Checking Running processes.."
  echo "----------------------------------------"
  }

  check_alert() {
   echo "checking system alerts.."
   DISK=$(df / | tail -1 | tr -s ' ' |  cut -d ' ' | tr -d '%')
   if [ $DISK -gt 80 ]
   then 
   echo "WARNING! Disk is $DISK% full!"
   else
      echo "OK! DISK usage is $DISK%"
      fi
     echo "-----------------------------------------"

   }

   check_memory
   check_disk
   check_processes
   check_alert

   echo "======================================"
   echo "  HEALTH CHECK COMPLETE!"
   echo "======================================"

### New commands Learned :
- tail -n -get last n lines
- tr -s -squeeze spaces
- tr -d -delete character
- cut -f5 -get specific column
- $() -store output in variables
- pipe | - connect command together
### Project built:
-healthmonitor.sh
 -check_memory()functions
 -check_disk() functions
 -check_processes() functions
 check_alert() functions
 Alerts when disk > 80%
