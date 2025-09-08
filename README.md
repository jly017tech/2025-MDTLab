<h1>Microsoft Deployment Toolkits Lab</h1>

<ul>
  <li>DHCP Server</li>
  <li>DNS Server</li>
  <li>Microsoft Deployment Toolkit</li>
  <li>Windows 11 Home</li>
  <li>PXE boot</li>
  <li>Lite Touch Windows PE is a boot image file where the IT professional use to deploy OS with Windows Deployment Service</li>
</ul>

<br>

<p>Youtube link:</p>

[![Watch the video](https://img.youtube.com/vi/GTKrgrngOTs/0.jpg)](https://www.youtube.com/watch?v=GTKrgrngOTs)


<br>
<hr>


<h2>Introduction</h2>

<p>
MDT stands for Microsoft Deployment Toolkit and it is deploys an operating system, an application, or a settings on the computers only running in Windows. As the video shows above, I have both virtual machines, domain controller and Windows 11 Client uninstall OS. Firsly, I setup DHCP Server so it automatically gives the IP address to the Windows 11 Home Client 2 virtual machine.
</p>

<br>

<hr>

<h2>Microsoft Deployment Toolkit Workbench</h2>

<img width="1290" height="642" alt="Screenshot from 2025-09-04 04-35-32" src="https://github.com/user-attachments/assets/71ef84ab-422b-483a-94ab-aff5f20d1679" />

<p></p>



<h2>Microsoft DeploymentToolkit using PXE boot</h2>

<img width="1331" height="865" alt="Screenshot from 2025-09-08 04-47-44" src="https://github.com/user-attachments/assets/f72324b8-5751-41fd-9f13-ec006c515590" />


<p>
  In this MDT lab, I use PXE boot to reimage a Windows 11 home on my second virtual machine.
  PXE stands for Preboot Execution Enviornment and it is part of the UEFI where it goes through netwowrk card adapter without need to plug in by USB drive to reimage operating system, such as, Windows, Linux, or MacOs. For example,  once the WDS activating, the second virtual machine that doesn't have operating system install gets automtically an IP address by DHCP server from the Domain Controller VM. 
</p>


<hr>

<h2>MDT Deployment page</h2>




<img width="858" height="653" alt="image" src="https://github.com/user-attachments/assets/29d29280-9360-4470-aeef-7b1bc9dd792a" />

<p>After the VM2 finally establish a connection from the DHCP server and WDS from Domain Controller, I went ahead go through each steps and finish deploying images.</p>

<hr>

<br>

<h2>CustomSetting.ini and Boostrap.ini</h2>

<img width="929" height="681" alt="image" src="https://github.com/user-attachments/assets/f99ee660-9f46-4fbc-9a3d-0a37f194795a" />

<hr>

<img width="929" height="681" alt="image" src="https://github.com/user-attachments/assets/5fae9483-b896-4d18-9823-f7cd2c819bd4" />

<p>
  I add some commands in both customSettinng.ini and Bootstrap.ini after opening with Notepad. In the customSetting, I put a comment for each sections so when i go back and know where to add or remove a command line from. For the other script, DeployRoot is a path file for getting from DCHuskyTech, name of the domain controller through folder call DeploymentShare$. Also, and the other lines are there for verifying HuskyTech.local credential as an aspiring IT professional
</p>

