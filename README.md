<p align="center">
<img src="https://i.imgur.com/sHWGzpY.png" alt="Azure Virtual Machines"/>
</p>

<h1>Creating Virtual Machines - Azure</h1>
This tutorial outlines the prerequisites and installation of creating virtual machines and resource groups in Microsoft Azure.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Resource Groups)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure Subscription/Free Trial

<h2>Installation Steps - Creating A Resource Group</h2>

<p>
  
- First things first, We are going to start in the Azure Portal. It should look something like this:

</p>
<p>
<img src="https://i.imgur.com/ioyIP6z.png" alt="Portal Home"/>
</p>

<br />

<p>
  
- Now lets create a Resource Group to create our virtual machine inside of. 
- Click on the resource group button on the Portal Home page or type in Resource Groups into the search bar.
- Once there, Click on the create button, and we will be taken to the creation page.

</p>
<p>
<img src="https://i.imgur.com/4mpRNbv.png" alt="Create Resouce Group"/>
</p>

<p>
  
- Now we are preseted with a few options, for the subscription we want to pick our subscription that we set up when creating our account. 
- The Resource Group Name is up to you, its simply what you want the group to be named, I went with Project_Demo for the sake of this tutorial. 
- Lastly pick a region thats relaible. US East or West is fine.
  
</p>
<p>
<img src=https://i.imgur.com/5ZoFTep.png alt="Create Resouce Group 2"/>
</p>
<p>
  
- Finally hit the Review+Create button at the bottom and once it finishes creating, you have made your first resource group!

</p>
<p>
<img src="https://i.imgur.com/zYvQKlM.png" alt="Create Resouce Group 3"/>
</p>
<p>
  
- If we head back to the Portal Home page then we are able to see our new resource group inside of the resource group tab. 

</p>
<p>
<img src="https://i.imgur.com/jPGudP5.png" alt="Create Resouce Group 4"/>
</p>

<br />

<h2>Installation Steps - Creating Our Virtual Machine</h2>

<p>

- The steps for creating a Virtual Machine are relatively the same as creating a Resource Group.
- First we are going to click on the virtual machine button on the azure home page and then hit create.
- On the dropdown choose the first option "Azure Virtual Machine."

<p>
<img src="https://i.imgur.com/hHYLDZM.png" alt="Create Virtual Machine"/>
</p>
<p>

- Now we are taken into the configuration for our Virtual Machine.
- Make sure that we are using the right Subscription. Select the same subscription that we used for the resource group.
- Pick a resource group to put our virtual machine inside of. (You can create the resource group here from scratch if you didnt in the steps above.) Pick the same one that we made earlier. For me it is Project_Demo.

<p>
<img src="https://i.imgur.com/Mmpqybt.png" alt="Create Virtual Machine 2"/>
</p>
<p>
  
- Make sure to name your virtual machine. Name it whatever you like.
- Pick the same region you picked for the resource group.
- Now pick the image that you would like the virtual machine to use. For this tutorial I just want windows 10 running so I picked that but you can also run windows servers, linux, etc...

<p>
<img src="https://i.imgur.com/FHEDPQ9.png" alt="Create Virtual Machine 3"/>
</p>
<p>
  
- Next we are going to select the size of the VM, which is essentially picking what components are in the PC. Make sure that it has at least 2 vcpus or it could run a little slow. If there is no option for 2 vcpus, hit the "See all sizes" button and you can pick it there.

<p>
<img src="https://i.imgur.com/E1bMW3v.png" alt="Create Virtual Machine 4"/>
</p>
<p>
  
- The last step before creating is picking a username and password to log into our Virtual Machine with. Pick something secure and write it down so you dont forget it. Anyone can use this to remote into the VM and we dont want that. Do not share the username or password with anyone you dont trust. 
- Lastly make sure you check the box for the licensing.

<p>
<img src="https://i.imgur.com/xCPoSvA.png" alt="Create Virtual Machine 5"/>
</p>
<p>
  
- Now hit the Review+Create button down at the bottom and create the virtual machine. (The other options like disk and networking do not matter to us in this tutorial since we are just creating a VM for personal use.)

<p>
<img src="https://i.imgur.com/8GdlVVG.png" alt="Create Virtual Machine 6"/>
</p>
<p>
  
- Give Azure some time to make the Virtual Machine, it can take a few minutes to create.
- Once it has created the VM, we will be able to see it in our resource group that we made previously. 

<p>
<img src="https://i.imgur.com/NcHlGNJ.png" alt="Create Virtual Machine 7"/>
</p>
<br />

<h2>How To Connect To The Virtual Machine</h2>

<p>
  
- Go back to the virtual machines page and there you will see the VM that you created. Take note of the Public IP Address. Either write it down somewhere or copy it. You will need to enter it alot so I recommend storing it.
- Make sure that the VM is running, it will say under status if it is or not. If it is not running then hit the "Start" button at the top and give it some time to boot up. 

<p>
<img src="https://i.imgur.com/JZgU2WI.png" alt="Using the VM"/>
</p>
<p>
  
- Once ready to connect to your VM, type "Remote Desktop Connection" into your windows search bar.
- Alternativevly hit the windows key on the keyboard (which is bottom left next to the "Control" button and "Alt" Button) and type it there.

<p>
<img src="https://i.imgur.com/ZvtTT8d.png" alt="Using the VM 2"/>
</p>
<p>
  
- You will be asked to enter in the computers public IP address, this is what we wanted to take note of earlier and can be found in the Virtual Machine page.
- Enter in the IP address and hit connect.

<p>
<img src="https://i.imgur.com/XYjxk8N.png" alt="Using the VM 3"/>
</p>
<p>
  
- You will be prompted to sign into the virtual machine now.
- Hit the "Use a different account" button at the bottom and now enter in the username and password that you created while setting up the virtual machine earlier.
- Then hit OK.

<p>
<img src="https://i.imgur.com/Gj5qWNJ.png" alt="Using the VM 4"/>
</p>
<p>
  
- You will be prompted again for security reasons
- Since we are the ones who created the VM and we know its safe, we will just ignore the warning and hit "Yes"

<p>
<img src="https://i.imgur.com/akKlwse.png" alt="Using the VM 5"/>
</p>
<p>
  
- After the VM signs you in for the first time windows will prompt you with some privacy settings.
- I reccomend turning off all of them however it is personal preference for these.

<p>
<img src="https://i.imgur.com/khEmZNL.png" alt="Using the VM 6"/>
</p>
<p>
  
- Finally after a long setup, we are in the machine and able to do whatever we need to do with it :)

<p>
<img src="https://i.imgur.com/kuqPMrL.jpeg" alt="Using the VM 7"/>
</p>

<h2>Cleanup/Exiting the VM</h2>

<p>
  
- Once you are done with the VM for the day to sign off, hit the X in the top middle of your screen and you will be prompted to disconnect.
- hit OK.

<p>
<img src="https://i.imgur.com/YxSvw6X.png" alt="Cleanup/Disconecting"/>
</p>
<p>
  
- If you are using a free trial of Azure it is important to make sure that you turn off your VM's if you know you will not be using them for the rest of the day or a while.
- VM's will cost you money by the hour if left running.

- Heres how to delete everything we just setup.
- First, lets head back to our resource groups.
- Since everything we created is inside of them, we can delete them and it will delete everything inside of them for us as well.
- Azure creates us a network group so you should have 2 resource groups.
- Select one of them by clicking on it.

<p>
<img src="https://i.imgur.com/0g4AsPs.png" alt="Cleanup/Disconecting 2"/>
</p>
<p>
  
- Once inside, click the "Delete resource group" button at the top

<p>
<img src="https://i.imgur.com/pBGnQ4Q.png" alt="Cleanup/Disconecting 3"/>
</p>
<p>
  
- You will then be asked to copy the name of the resource group and paste it into the text box at the bottom.
- This is to confirm that you want to delete the resource group. Hit delete and give Azure some time to delete everything for you.
- Do the same process for the network group that was created and any other resource groups that you created.

<p>
<img src="https://i.imgur.com/qarY7Lw.png" alt="Cleanup/Disconecting 4"/>
</p>
















