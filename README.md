# Auto Node Start - Readme

NOTE: You should have a working remme installation before you perform these next steps.

The communitytools script creates 4 scripts:

start.sh - starts the master node in background mode
stop.sh - stops the masternode
check.sh - checks the operations of your node using standard http
checkssl.sh - checks the operations of your node using standard SSL.  For this to work you must have completed the SSL section of the advanced user guide

1) Copy and paste the whole script into your command prompt or putty. Let it settle, then press enter.
2) Once you run the script, perform a reboot of your server by either using the reboot command or use your VPS restart server command.

You can see these files by using the ls command.  Let me show you how.

Connect to the server using ssh. Once you are connected use:
##---- code start ---
cd /home/remmecommunity 
ls
##---- code end -----
You will see the files.

Try all four of the scripts

stop.sh
start.sh
check.sh
checkssl.sh

You could just call the absolute path of the scripts like so

/home/remmecommunity/start.sh
/home/remmecommunity/stop.sh
/home/remmecommunity/check.sh
/home/remmecommunity/checkssl.sh

When you reboot the server it will automatically run /home/remmecommunity/start.sh after 3 seconds

Catch me on telegram if you need anything!
