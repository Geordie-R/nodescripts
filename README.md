<h1>Community Tools - Readme </h1>

<h3>NOTE: You should have a working remme installation before you perform these next steps.</h3>

<p>The communitytools script creates 4 scripts:</p>
<ul>
<li>start.sh - starts the master node in background mode</li>
<li>stop.sh - stops the masternode</li>
<li>check.sh - checks the operations of your node using standard http</li>
<li>checkssl.sh - checks the operations of your node using standard SSL.  For this to work you must have completed the SSL section of the advanced user guide</li><ul>
<p>
1) Copy and paste the whole script into your command prompt or putty. Let it settle, then press enter.<br />
2) Once you run the script, perform a reboot of your server by either using the reboot command or use your VPS restart server command.<br />
  </p>
<p>You can see these files by using the ls command.  Let me show you how.</p>
<p>
Connect to the server using ssh. Once you are connected use:
##---- code start ---
cd /home/remmecommunity 
ls
##---- code end -----
  </p><br />
You will see the files.
<br />
<p>Try all four of the scripts
<ul>
  <li>stop.sh</li>
 <li>start.sh</li>
 <li>check.sh</li>
 <li>checkssl.sh</li>
</ul>
<p>
You could just call the absolute path of the scripts like so</p>
<ul>
  <li>/home/remmecommunity/start.sh</li>
  <li>/home/remmecommunity/stop.sh</li>
  <li>/home/remmecommunity/check.sh</li>
  <li>/home/remmecommunity/checkssl.sh</li>
</ul>

<p>When you reboot the server it will automatically run /home/remmecommunity/start.sh after 3 seconds</p>

<p style='weight:bold;'>Catch me on telegram if you need anything!</p>
