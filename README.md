<h1>Community Tools - Readme </h1>

<h3>NOTE: You should have a working remme installation before you perform these next steps.</h3>

<p>The communitytools script creates 4 scripts:</p>
<ul>
<li>start.sh - starts the master node in background mode</li>
<li>stop.sh - stops the masternode</li>
<li>check.sh - checks the operations of your node using standard http</li>
<li>checkssl.sh - checks the operations of your node using standard SSL.  For this to work you must have completed the SSL section of the advanced user guide</li>
 <li>Install.sh - left over from install for reinstallation / debugging.</li>
</ul>
<p>
 
 ``` 
## Parameters Start ##
export REMME_CORE_RELEASE="0.7.0-alpha"
export DOMAIN_OR_IP="testme.com"
export INSTALL_LOCATION="/home/remmecommunity/"
## Parameters End ##
## Lets make a directory called remmecommunity and not care if it exists
mkdir -p $INSTALL_LOCATION		
## Lets make the permissions relaxed for group members and the user who created it read,write and execute privs
chmod 770 $INSTALL_LOCATION
## Now download the main script
curl https://raw.githubusercontent.com/Geordie-R/nodescripts/master/communitytools | sudo tee /home/remmecommunity/install.sh > /home/remmecommunity/install.sh
## Do some find and replaces
sudo -i sed -i "s/REPLACED_YOURDOMAINORIP/$DOMAIN_OR_IP/g" /home/remmecommunity/install.sh
sudo -i sed -i "s/REPLACED_REMMECORERELEASE/$REMME_CORE_RELEASE/g" /home/remmecommunity/install.sh
sudo -i sed -i "s/REPLACED_INSTALLLOCATION/$INSTALL_LOCATION/g" /home/remmecommunity/install.sh
sudo chmod 770 /home/remmecommunity/install.sh
/home/remmecommunity/install.sh
 
 ```
  
  
<ol><li>Copy and paste the code above into your putty window or command prompt</li>
  <li>Change the parameters at the top in the parameters section.  Change
   
   ```
   export REMME_CORE_RELEASE=0.7.0-alpha
   
   ``` 
   
   to whatever version of Remme Core you have installed.  I will always update this script once new versions become available. e.g. if remme release a 0.8.0-alpha then that line would become 
   ```
   export REMME_CORE_RELEASE=0.8.0-alpha
   ```
   
   </li>
  <li>Change the next line further down:
  
  ```
  export DOMAIN_OR_IP=your-domain-or-ip-here.com
  ```
  
  .  If you have a domain name on your node type your domain name in place of your-domain-or-ip-here.com. if you had a domain called mynoderules.com then this would become 
  ```
  export DOMAIN=mynoderules.com
  ``` 
  . If you have not bought a domain name input your ip address instead. So this would become 
  ```
  DOMAIN_OR_IP=123.123.123.123
  ``` 
  where those numbers represent your nodes ip address. Be sure to change it.</li>
<li>Once that is done copy all of the code in notepad by going to Edit > Select All then Edit > Copy.  Then paste it into your command prompt or whichever terminal you are using e.g. putty.</li>
  
  <li>Perform a reboot of your server by either using the 'reboot' command or use your VPS restart server command</li>
<li>Close any command prompt or terminal windows and reconnect to your node</li>
</ol>
  </p>
  
  <p> Thats the install complete.</p>
  
  
<p>You can see these files by using the ls command.  Let me show you how.</p>
<p>
  
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
Another way to call the scripts is to call the absolute path of the scripts like so so that its just one command.</p>

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
