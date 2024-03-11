**Laura Cobham GEOM99 Technical Log**

**ArcGIS Server on GCP**//
2024/03/06 11pm start, 12am end (1 hour spent)
During this session I watched and recreated Shawn's video from this link: https://youtu.be/dyFeyBX9jIY, creating my own GCP server

First go to the Google CLoud website at: console.cloud.google.com and naviagte to Compute Engine - VM instances from the top left.
Create Instance, name it (eg arcgisserver), and go to the 'Boot disk' section. Click 'Change' and change the 'source project for image' in 'custom images' to the current project, click select.
Allow 'HTTP traffic' and 'HTTPS traffic' and choose 'create'.
Go to 'set up firewall rules' and name the rule (eg flemingrdp444).
Change target to 'all instances in the network'.
Enter 0.0.0.0/0 in the 'source IPv4 ranges' section. Add ports 444 and 6443 to the ports section under 'TCP' (444 makes it work at Fleming).
Set a new Windows password by clicking the dropdown arrow next to 'RDP', making the username 'student'. The password will auto-generate (x}9Yo[ifHyX;E1l).

Search 'mstc' in your computer's search bar and enter the IP address from the 'External IP' section of the GCP with ':444' on the end.
For credentials, click more choices if the user is already filled and enter student as the username and 'x}9Yo[ifHyX;E1l' as the password.
A certificate warning will come up, choose yes.
**IMPORTANT** clicking 'X' on the virtual desktop will not shut it down, it will still charge you. To fully shut it down, go back to the Google Cloud website and choose 'Stop' from the 3 dots dropdown menu and wait for it to show the grey stop button.

To go to the manager site type in: https://IPADDRESS:6443/arcgis/manager/, replacing IDADDRESS with the new randomly generated IP address from the 'External IP' section of the GCP.
Log in with siteadmin and the password from the checklist Week 7/8 GEOM99 checklist.

**Using AGOL and ArcGIS Server on GCP together**//
2024/03/10 8:30pm start, ___ end (total)
During this session I relaunched the GCP that I created last time and used it to publish the items inside onto ArcGIS Online using multiple methods.

To relaunch the GCP server, go to the Google Cloud website (https://console.cloud.google.com), go to the top left and click Compute Engine - VM instances.
Then press the 3 dots next to your server and select resume/play on the server you want to resume.
Then search 'mstc' in your computer's search bar and enter the IP address from the 'External IP' section of the GCP with ':444' on the end.
For credentials, click more choices if the user is already filled and enter student as the username and 'x}9Yo[ifHyX;E1l' as the password.
A certificate warning will come up, choose yes.
The virtual desktop is now launched, come back to this section every time you want to relaunch it.

To check the server is replying, enter the new randomly generated IP address from the 'External IP' section of the GCP into the search bar. To see the directory and check the server is up and running, enter https://IPADDRESS/arcgis/rest/services into the search bar replacing the IDADDRESS with the new randomly generated IP address from the 'External IP' section of the GCP.

After recreating those steps:
-Sign into AGOL, go to Content and choose add item
-To add items from the Server as a feature layer choose add URL and add: https://*IPADDRESS/arcgis/rest/services/SampleWorldCities/MapServer/0 (*insert new IP that is generated each time GCP is turned on)
-To add items from the Server as a map image layer (ie a picture of the data) choose URL and add: https://*IPADDRESS/arcgis/rest/services/SampleWorldCities/MapServer (*insert new IP that is generated each time GCP is turned on)
