<p align="center">
<img src="https://i.imgur.com/5QFqQyS.png" alt="Azure Cloud Logo"/>
</p>

<h1>Azure Virtual Machine Deployment with RDP</h1>
This tutorial outlines how to deploy a Windows virtual machine in Microsoft Azure using the Azure Portal and connect to it with Remote Desktop Protocol (RDP).<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Create an Azure VM and Connect with RDP](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines / Compute)
- Azure Portal (Web GUI)
- Remote Desktop Connection (RDP)
- Virtual Network / Network Security Group (NSG)

<h2>Operating Systems Used</h2>

- Windows 10 / 11 (local client machine)
- Windows 10 / Windows Server (Azure virtual machine)

<h2>List of Prerequisites</h2>

- An active Microsoft Azure subscription
- A local computer with Internet access
- Remote Desktop Connection installed (built into Windows)
- Web browser to access the Azure Portal
- Basic understanding of logging in and navigating Azure Portal

<h2>Deployment Steps</h2>

<p>
<img src="https://i.imgur.com/AAAAAAAA.png" height="80%" width="80%" alt="Azure Portal Home"/>
</p>
<p>
<b>Step 1: Log in to the Azure Portal</b><br />
Navigate to <a href="https://portal.azure.com" target="_blank">https://portal.azure.com</a> and sign in with your Azure account. Once logged in, you’ll land on the Azure Portal dashboard where you can create and manage resources.
</p>
<br />

<p>
<img src="https://i.imgur.com/BBBBBBBB.png" height="80%" width="80%" alt="Create Virtual Machine"/>
</p>
<p>
<b>Step 2: Create a New Virtual Machine</b><br />
From the Azure Portal, click on <b>“Virtual machines”</b> in the left menu, then click <b>“Create”</b> &rarr; <b>“Azure virtual machine”</b>.  
On the <b>Basics</b> tab, choose or create a <b>Resource group</b>, give your VM a name, select a <b>Region</b> close to you, and choose the <b>Image</b> (for example, Windows 10 or Windows Server). Select a VM size that fits this lab (e.g., B1s or similar).
</p>
<br />

<p>
<img src="https://i.imgur.com/CCCCCCCC.png" height="80%" width="80%" alt="Administrator Account and Inbound Ports"/>
</p>
<p>
<b>Step 3: Configure Administrator Account and RDP Access</b><br />
On the same page, create an <b>Administrator username</b> and a strong <b>Password</b> for your VM (you’ll use this later to log in).  
Under <b>Inbound port rules</b>, make sure <b>“Allow selected ports”</b> is chosen and check <b>RDP (3389)</b>. This opens the RDP port so you can connect remotely to the VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/DDDDDDDD.png" height="80%" width="80%" alt="Review and Create VM"/>
</p>
<p>
<b>Step 4: Review and Create the Virtual Machine</b><br />
Click through the remaining tabs (Disks, Networking, Management) and leave the default options for this lab unless you need to change something specific.  
When you reach the <b>“Review + create”</b> tab, Azure will validate your configuration. If validation succeeds, click <b>“Create”</b>.  
Azure will start deploying your virtual machine. This process may take a few minutes.
</p>
<br />

<p>
<img src="https://i.imgur.com/EEEEEEEE.png" height="80%" width="80%" alt="VM Overview and Public IP Address"/>
</p>
<p>
<b>Step 5: Locate the VM and Public IP Address</b><br />
Once deployment completes, click <b>“Go to resource”</b> to open the VM’s overview page.  
On the <b>Overview</b> blade, you’ll see details about the VM, including its <b>Public IP address</b>. Copy this IP address—you’ll use it to connect via Remote Desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/FFFFFFFF.png" height="80%" width="80%" alt="Remote Desktop Connection"/>
</p>
<p>
<b>Step 6: Connect to the VM Using RDP</b><br />
On your local Windows computer, open <b>Remote Desktop Connection</b> (you can search for “Remote Desktop” in the Start menu).  
Paste the VM’s <b>Public IP address</b> into the <b>Computer</b> field and click <b>Connect</b>.  
When prompted, enter the <b>username</b> and <b>password</b> you created for the VM in Step 3. Accept any certificate warning.  
If everything is configured correctly, you will be logged in to your Azure virtual machine desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/GGGGGGGG.png" height="80%" width="80%" alt="Deleting Resource Group"/>
</p>
<p>
<b>Step 7: Clean Up (Delete Resources)</b><br />
To avoid unnecessary charges in Azure, return to the Azure Portal and navigate to <b>Resource groups</b>.  
Locate the resource group you created for this VM, click on it, and then click <b>“Delete resource group”</b>. Type the name to confirm and delete all associated resources (VM, disk, network, public IP, etc.).
</p>
<br />

<h2>Summary</h2>
In this lab, we created a Windows virtual machine in Microsoft Azure using the Azure Portal, enabled RDP access by opening port 3389, connected to the VM from a local computer using Remote Desktop, and finally cleaned up the resources when finished. This demonstrates core cloud skills such as provisioning compute resources, basic networking, and remote administration in Azure.
