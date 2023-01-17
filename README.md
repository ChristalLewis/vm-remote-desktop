<p align="center">
<img src="" alt=""/>
</p>

<h1>Creating Virtual Machines and Using Remote Desktop Connection</h1>
This tutorial outlines how to create virtual machines in Azure and use the remote desktop connection to gain access.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a free Microsoft Azure account. Find the steps [here](https://learn.microsoft.com/en-us/training/modules/create-an-azure-account/)
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/lP7ML9j.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1. Once you are logged into your Azure account, go to the search bar and type "Resource Group". Then select the gray highlighted words "Resource group" with a left click of your mouse/touchpad.
</p>
<br />

<p>
<img src="https://i.imgur.com/pUGr1Zj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. From the menu in the top left hand corner, choose "+ create" (by left clicking) in order to set up a new resource group.
</p>
<br />

<p>
<img src="https://imgur.com/mzwwHUJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. On this screen, we are going to fill out the form. (a) Choose the azure subscription you want to use. (b) Name the resource group (I recommend using a name that makes sense for the project). (c) Choose the region you are located in. (d) Click "Next:Tags>".
</p>
<br />
<p>
<img src="https://imgur.com/dAoI7Lh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. (a) In the name area, put your name. (b) In value, put your role/job. (c) Click "Next:Review+create>".
</p>
<br />

<p>
<img src="https://imgur.com/jjubX1Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5. When you see the words Validation passed with the green circle and white check inside in front, click "Create" (at the bottom left of the screen).
</p>
<br />

<p>
<img src="http://i.imgur.com/UGf4YQE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. This process may take some time to create the resource group. When your screen looks like this (except with your chosen resource group name), your resource group is created and ready to use.
</p>
<br />
<p>
<img src="https://imgur.com/aBebBlR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. Now we are going to create our virtual machine. Go to the search bar and type "Virtual Machine". Then select the gray highlighted words "Virtual machines" with a left click of your mouse/touchpad. 
</p>
<br />

<p>
<img src="https://imgur.com/p9Owzsv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. From the menu in the top left hand corner, choose "+ create" (by left clicking) in order to set up a new virtual machine. Choose "Azure virtual machine" from the drop down menu.
</p>
<br />

<p>
<img src="https://imgur.com/ctaNZRW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
9. Now we have to fill out the specific information for the virtual machine we are creating. (a) Choose the same subscription and resource group name you choose when creating the resource group. (b) Choose a virtual machine name (this name must be original and I recommend you pick a name relevant to your project). (c) Choose your region again (it should be the same as the region you chose when creating the resource group). (d) Leave the Availability options and Availability zone chosen for you. (e) Scroll down and continue to fill out the form.
</p>
<br />
<p>
<img src="https://imgur.com/cE0cY4u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
10. Fill out this screen so it matches the picture exactly (As you learn more and have other needs, you will change some of these options). Scroll down and continue to fill out the form.
</p>
<br />

<p>
<img src="https://imgur.com/iKTodJR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
11. (a) Choose your username. (b) Choose Your password and confirm it (follow the guidelines for the passwords). (c) Leave the Public and Select inbound port fields the same as you see in the picture. (d) Scroll down and continue to fill out the form. 
*REMINDER: KEEP TRACK OF THE USERNAME AND PASSWORD, YOU WILL NEED IT LATER*
</p>
<br />

<p>
<img src="https://imgur.com/E6cdZBX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
12. (a) Check the box under the Licensing area. (b) Click "Next:Disks>". 
</p>
<br />
<p>
<img src="https://imgur.com/miBCeUU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
13. (a) In the top menu, choose the "Networking" tab (you know you're in the right menu when the words "Networking" has a gray background). (b) Take note of the Network Interface settings. (c) Click the "Review+create" button in the bottom left corner.
</p>
<br />

<p>
<img src="https://imgur.com/2mNeKJs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
14. When you see the words Validation passed with the green circle and white check inside in front, click "Create" (at the bottom left of the screen). 
</p>
<br />

<p>
<img src="https://imgur.com/X9txysm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
15. This process may take some time to create the virtual machine. When your screen says "Your deployment is complete" and looks like the picture above, your virtual machine is created and ready to use. 
</p>
<br />
<p>
<img src="https://imgur.com/HnPnJkD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
16. Now we are going to check the networking. Go to the search bar and type "network watcher". Then select the gray highlighted words "Network Watcher" with a left click of your mouse/touchpad. 
</p>
<br />

<p>
<img src="https://imgur.com/u9qXobr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
17. On the left hand menu (under "Monitoring"), click "Topology".
</p>
<br />

<p>
<img src="https://imgur.com/p8w5mtn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
18. Choose the subscription, resource group, and virtual network you created. If your screen looks like the picture above, you have successfully set up your virtual machine within the resource group you created.
</p>
<br />
<p>
<img src="https://imgur.com/qRGCFbf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
19. Now we are going to connect remotely to the virtual machine we created. In the search bar at the bottom of your screen, type "Remote Desktop Connection". Then select "Open".
*FOR THOSE WITH APPLE DEVICES, DOWNLOAD THE REMOTE DESKTOP APP AND OPEN IT*
</p>
<br />

<p>
<img src="https://imgur.com/6cvLb5L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
20. (a) Select the virtual machine (in the Azure website). (b) Copy the Public IP address. (c) Paste the IP address in the field labeled "Computer". (d) Click "Connect".
</p>
<br />

<p>21
<img src="https://imgur.com/Pnp3Lam.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />
<p>22
<img src="https://imgur.com/8V6ZeN4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />

<p>22a
<img src="https://imgur.com/RFKVLEM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />
<p>22b
<img src="https://imgur.com/D0BtYWC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />

<p>22c
<img src="https://imgur.com/i4lqtPG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet
</p>
<br />

<p>23
<img src="https://imgur.com/ABUpWwm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet
</p>
<br />

<p>24
<img src="https://imgur.com/Y0vUp6B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />

<p>25
<img src="https://imgur.com/Xk20i7E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />
<p>26
<img src="https://imgur.com/kwj7gnL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, 
</p>
<br />

<p>27
<img src="https://imgur.com/CooRlaC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet
</p>
<br />



