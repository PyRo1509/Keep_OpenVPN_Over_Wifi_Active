#Keep_OpenVPN_Over_Wifi_Active
------

For use with an OpenVPN client that is connected by wifi. Rarely the connection might drop. The script tests for when this happens. It then diagnoses the issue and repairs it.

After getting the script run it once. This will create the config file.
Change remote_ip and wifi_ap. Other settings will work for Default.

Useage:

Always running from startup:

```
crontab -e
* * * * * /bin/bash /home/{HOME}/Keep_OpenVPN_Over_Wifi_Active/Keep_OpenVPN_Over_Wifi_Active
```
This will run every minute. It checks to see if it is currently running, if so it quits.


```
screen
sudo bash Keep_OpenVPN_Over_Wifi_Active
```
This is a good way to debug as output is defaulted to the terminal.
