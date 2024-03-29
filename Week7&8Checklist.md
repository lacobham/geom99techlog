# Laura Cobham GEOM99 Technical Log 
(For start/end times, time spent, resources and next steps, see the Excel time log. This file is the outcomes)

Formatting: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## ArcGIS Server on GCP

2024/03/06

During this session I watched and recreated Shawn's video from this link: https://youtu.be/dyFeyBX9jIY, creating my own GCP server
1. First go to the Google Cloud website at: console.cloud.google.com and naviagte to Compute Engine - VM instances from the top left.
1. Create Instance, name it (eg arcgisserver), and go to the 'Boot disk' section. Click 'Change' and change the 'source project for image' in 'custom images' to the current project, click select.
1. Allow 'HTTP traffic' and 'HTTPS traffic' and choose 'create'.
1. Go to 'set up firewall rules' and name the rule (eg flemingrdp444).
1. Change target to 'all instances in the network'.
1. Enter 0.0.0.0/0 in the 'source IPv4 ranges' section. Add ports 444 and 6443 to the ports section under 'TCP' (444 makes it work at Fleming).
1. Set a new Windows password by clicking the dropdown arrow next to 'RDP', making the username 'student'. The password will auto-generate (x}9Yo[ifHyX;E1l).
1. Search 'mstc' in your computer's search bar and enter the IP address from the 'External IP' section of the GCP with ':444' on the end.
1. For credentials, click more choices if the user is already filled and enter student as the username and 'x}9Yo[ifHyX;E1l' as the password.
1. A certificate warning will come up, choose yes.
**IMPORTANT** clicking 'X' on the virtual desktop will not shut it down, it will still charge you. To fully shut it down, go back to the Google Cloud website and choose 'Stop' from the 3 dots dropdown menu and wait for it to show the grey stop button.

1. To go to the manager site type in: https://IPADDRESS:6443/arcgis/manager/, replacing IDADDRESS with the new randomly generated IP address from the 'External IP' section of the GCP.
  1. Log in with siteadmin and the password from the checklist Week 7/8 GEOM99 checklist.

## Using AGOL and ArcGIS Server on GCP together

2024/03/10

During this session I relaunched the GCP that I created last time and used it to publish the items inside onto ArcGIS Online using multiple methods. I also created this technical log up to the end of this step.

1. To relaunch the GCP server, go to the Google Cloud website (https://console.cloud.google.com), go to the top left and click Compute Engine - VM instances.
1. Then press the 3 dots next to your server and select resume/play on the server you want to resume.
1. Then search 'mstc' in your computer's search bar and enter the IP address from the 'External IP' section of the GCP with ':444' on the end.
1. For credentials, click more choices if the user is already filled and enter student as the username and 'x}9Yo[ifHyX;E1l' as the password.
1. A certificate warning will come up, choose yes.
1. The virtual desktop is now launched, come back to this section every time you want to relaunch it.
1. To check the server is replying, enter the new randomly generated IP address from the 'External IP' section of the GCP into the search bar. To see the directory and check the server is up and running, enter https://IPADDRESS/arcgis/rest/services into the search bar replacing the IDADDRESS with the new randomly generated IP address from the 'External IP' section of the GCP.

After recreating those steps:
1. Sign into AGOL, go to Content and choose add item
1. To add items from the Server as a feature layer choose add URL and add: https://*IPADDRESS/arcgis/rest/services/SampleWorldCities/MapServer/0 (*insert new IP that is generated each time GCP is turned on)
1. To add items from the Server as a map image layer (ie a picture of the data) choose URL and add: https://*IPADDRESS/arcgis/rest/services/SampleWorldCities/MapServer (*insert new IP that is generated each time GCP is turned on)

## Publish Canada service to your own GCP VM

During this session, I published the Canada map data on the server from the VM.
1. To publish the Canada map onto the server from the VM, I first copied the data from the zip folder on the desktop to the gisworkspace folder on the C drive.
1. Then open ArcGIS Pro on the local computer and add a new ArcGIS server connection.
1. Click yes when warned about the certificate.
1. For the server URL enter https://IPADDRESS:6443/arcgis (IPADDRESS regenerates every time on Google Cloud website - External IP)
    1. Username: siteadmin
    1.Password: In the Week 7/8 checklist
1. Then, create a new folder on local laptop with same canada data in the same location as it was on the VM.
1. Then naviagte to the server connection and choose publish, then publish as map service.
1. Analyze and fix any errors (assign unique numeric IDs, register data source), then publish.

2. Refer to Shawn's video on this for more: https://www.youtube.com/watch?v=nIRlZN9ECwY&t=776s.
