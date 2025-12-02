<p align="center">
  <img src="https://i.imgur.com/5QFqQyS.png" alt="Azure Cloud Logo"/>
</p>

<h1>Azure Virtual Machine Deployment with RDP</h1>
This tutorial outlines how to deploy a Windows virtual machine in Microsoft Azure using the Azure Portal and connect to it using Remote Desktop Protocol (RDP).

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines)</li>
  <li>Azure Portal</li>
  <li>Remote Desktop Connection (RDP)</li>
  <li>Virtual Network</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 / 11 (local computer)</li>
  <li>Windows 10 / Windows Server (Azure VM)</li>
</ul>

<h2>Prerequisites</h2>
<ul>
  <li>Active Microsoft Azure subscription</li>
  <li>Computer with internet access</li>
  <li>Remote Desktop Connection installed</li>
  <li>Ability to navigate Azure Portal</li>
</ul>

<h2>Deployment Steps</h2>

<h3>Step 1: Log in to the Azure Portal</h3>
<p>Screenshot: <a href="https://imgur.com/a/XUfxshS" target="_blank">View Image</a></p>
<p>Navigate to the Azure Portal and sign in with your Microsoft Azure account.</p>

<h3>Step 2: Create a New Virtual Machine</h3>
<p>Screenshot: <a href="https://imgur.com/a/sDDy51L" target="_blank">View Image</a></p>
<p>Click “Virtual Machines” → “Create” → “Azure virtual machine.” Choose a resource group, name, region, and image.</p>

<h3>Step 3: Configure Administrator Account and RDP Access</h3>
<p>Screenshot: <a href="https://imgur.com/a/3bBPlMv" target="_blank">View Image</a></p>
<p>Set a username and password, then allow RDP (port 3389) under inbound port rules.</p>

<h3>Step 4: Review and Create the Virtual Machine</h3>
<p>Screenshot: <a href="https://imgur.com/a/fG7e6dY" target="_blank">View Image</a></p>
<p>Review your VM settings and click “Create.” Azure will begin deploying the virtual machine.</p>

<h3>Step 5: Get the Public IP Address</h3>
<p>Screenshot: <a href="https://imgur.com/a/jdeLoEm" target="_blank">View Image</a></p>
<p>When deployment completes, open the VM resource page and copy its public IP address.</p>

<h3>Step 6: Connect Using RDP</h3>
<p>Screenshot 1: <a href="https://imgur.com/a/2PElKta" target="_blank">View Image</a></p>
<p>Screenshot 2: <a href="https://imgur.com/a/jb7fQ1d" target="_blank">View Image</a></p>
<p>Open Remote Desktop Connection, paste the VM’s public IP, and log in using the credentials you created.</p>

<h3>Step 7: Clean Up Resources</h3>
<p>Screenshot: <a href="https://imgur.com/a/SBuED3h" target="_blank">View Image</a></p>
<p>Delete your resource group to remove all associated resources and avoid extra charges.</p>

<h2>Summary</h2>
<p>
This lab demonstrates how to deploy a Windows virtual machine in Azure, enable RDP access, connect remotely, and clean up cloud resources. It showcases essential cloud skills such as virtual machine deployment, networking, authentication, and resource management.
</p>
