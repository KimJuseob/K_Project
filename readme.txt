1. Please put the NVR and PC on the 192.168.1.xxx network  (note: must be 192.168.1.xxxx )
2. Please telent the NVR , use the NVR IP.  eg: telnet 192.168.1.100
3. Please input user and password. user: root    passwd: rsfd1s*
4. Please input command: dd if=/dev/zero of=/dev/mtdblock3 bs=1M count=2   
5. Please input command: sync
6. Please input command: reboot

7. Please get the attachment file app_V170828_N5332_M . then copy to the USB. 
8. Please login the NVR again. the NVR ip is will changed to 192.168.1.99.  so please input: telent 192.168.1.99 to login in 
   if you login in the NVR, please input command:
    mkdir /dev/tmp1  ;
    mount /dev/udisksda1  /dev/tmp1  or mount /dev/udisksdb1  /dev/tmp1
9. Please input command:  ls -l  /dev/tmp1     to get app_V170828_N5332_M size
10. Please input command: dd if=./app_V170828_N5332_M of=/dev/mtdblock3 bs=10121216 count=1         (10121216 = app_V170828_N5332_M size)
11. Please input command: sync
12. Please input command: reboot

13. Please use N5332_V170503V170512V170726V170824V170613V170821_W.sw that I send to you to upgrade by USB.

 