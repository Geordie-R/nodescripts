# Auto Node Start - Readme
Once you run the script, perform a reboot of your server and log back in by using the reboot command or use your VPS restart server command.

You will now have two files now at /home/remmecommunity
start.sh
stop.sh

Running ./home/remmecommunity/start.sh will start your node if it hasnt already started if you have stopped it.
Running ./home/remmecommunity/stop.sh will stop your node if it is currently running.

When you reboot the server it will automatically run /home/remmecommunity/start.sh

IF it doesn't, well, can't say im surprised this isn't really to be ran without first taking a snapshot as I'm still polishing the code.
