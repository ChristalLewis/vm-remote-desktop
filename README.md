<p align="center">
<img src="" alt=""/>
</p>

<h1>Creating Virtual Machines and Using Remote Desktop Connection</h1>
This tutorial outlines how to create virtual machines (computer and server) in Azure and use the remote desktop connection to gain access.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop 

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Linux (Ubuntu)
- Windows Server 2022 Datacenter

<h2>List of Prerequisites</h2>

- For absolute beginners with zero knowledge, I suggest Youtube/Google terms like "virtual machines" and "remote desktop connection"
- Create a free Microsoft Azure account. Find the steps [here](https://learn.microsoft.com/en-us/training/modules/create-an-azure-account/)
- Login to your free account.

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
6. This process may take some time to create the resource group. When your screen looks like the picture above (except with your chosen resource group name), your resource group is created and ready to use.
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

<p>
<img src="https://imgur.com/Pnp3Lam.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
21. In the user and password sections, put the username and password you created in step 11. Check the "remember me" box ONLY if you are using your personal computer. Then click "OK".
</p>
<br />
<p>
<img src="https://imgur.com/8V6ZeN4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
22. Click "OK". 
</p>
<br />

<p>
<img src="https://imgur.com/RFKVLEM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
23. Choose no for all of the privacy settings (your screen should look like the picture above. Click "Accept".
</p>
<br />
<p>
<img src="https://imgur.com/D0BtYWC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
24. You have successfully secured a remote desktop connection to your virtual machine if your screen looks like the picture above (except the IP address at the top of the screen could be different).
</p>
<br />

<p>
<img src="https://imgur.com/i4lqtPG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
25. Sometimes, it can get confusing which screen is the virtual machine or your actual screen. The virtual machine will have the blue bar at the top of the screen (as shown in the picture above). To go to your computer desktop, click the minimize icon ( _ ). Click "_".
</p>
<br />

<p>
<img src="https://imgur.com/ABUpWwm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
26. Now we are going to create another virtual machine (with a linux OS). (a) Follow steps 7-9 (excpet the virtual machine name has to be different than the first one) to create another virtual machine. (b) Fill out the form just like the picture in step 10 (except in the image field, pick a linux Operating System). (c) In the authentication type field, select the "Password" bubble (like in the picture above). (d) For the username and password, you can use the same info as the first virtual machine (make sure to save this info). (e) Click the "Review+create" button in the bottm left hand of the screen.
</p>
<br />

<p>
<img src="https://imgur.com/Y0vUp6B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
27. Follow the steps 16 through 18 to check the networking of the two virtual machines (computers) you created. Your screen should look like the picture above. 
</p>
<br />

<p>
<img src="https://imgur.com/Xk20i7E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
28. If you want to create a virtual server instead of a virtual computer, follow step 26 to create a virtual machine (except in the image field, choose "Windows Server" from the dropdown menu). Keep in mind, virtual servers and virtual computers are both virtual machines.
</p>
<br />
<p>
<img src="https://imgur.com/kwj7gnL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
29. When creating the virtual server, check both boxes under the "Licensing" section (like in the picture above). Then click the "Review+create" button in the bottom left of the screen.
</p>
<br />

<p>
<img src="https://imgur.com/CooRlaC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
30. To check the networking, follow steps 16 through 18. The picture above shows the two virtual computers and the virtual server created within the resource group.
</p>
<br />



