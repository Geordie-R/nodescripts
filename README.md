<h1>Community Tools - Readme </h1>

<h3>NOTE: You should have a working remme installation before you perform these next steps.</h3>

<p>The communitytools script creates 4 scripts:</p>
<ul>
<li>start.sh - starts the master node in background mode</li>
<li>stop.sh - stops the masternode</li>
<li>check.sh - checks the operations of your node using standard http</li>
<li>checkssl.sh - checks the operations of your node using standard SSL.  For this to work you must have completed the SSL section of the advanced user guide</li></ul>
<p>
<ol><li>Copy and paste the whole script into your command prompt or putty. Let it settle, then press enter</li>
<li>Once you run the script, perform a reboot of your server by either using the reboot command or use your VPS restart server command<li></ol>
  </p>
<p>You can see these files by using the ls command.  Let me show you how.</p>
<p>
Connect to the server using ssh. Once you are connected use:
  
```
cd /home/remmecommunity 
ls
```
  </p>
You will see the files.
<br />
<p>Try all four of the scripts
  
  ```
  stop.sh
  ```
  
  ```
  start.sh
  ```
  
  ```
  check.sh
  ```
  
  ```
  checkssl.sh
  ```
<p>
You could just call the absolute path of the scripts like so</p>

```
/home/remmecommunity/start.sh
```

```
/home/remmecommunity/stop.sh
```

```
/home/remmecommunity/check.sh
```

```
/home/remmecommunity/checkssl.sh
```


<p>When you reboot the server it will automatically run the following code below after 3 seconds</p>
  
  ```
  /home/remmecommunity/start.sh
  ```
<p style='weight:bold;'>Catch me on telegram if you need anything!</p>
