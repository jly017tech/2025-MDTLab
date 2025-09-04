<h1>MDT Lab</h1>

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


<h2>Intro</h2>

<p>
MDT stands for Microsoft Deployment Toolkit and it is deploys an operating system, an application, or a settings on the computers only running in Windows. As the video shows above, I have both virtual machines, domain controller and Windows 11 Client uninstall OS. Firsly, I setup DHCP Server so it automatically gives the IP address to the Windows 11 Home Client 2 virtual machine.
</p>

<br>

<h2>Microsoft DeploymentToolkit using PXE boot</h2>

<p>
  In this MDT lab, I use PXE boot to reimage a Windows 11 home on my second virtual machine.
  PXE stands for Preboot Execution Enviornment and it is part of the UEFI where it goes through netwowrk card adapter without need to plug in by USB drive to reimage operating system, such as, Windows, Linux, or MacOs. For example,  once the WDS activating, the second virtual machine that doesn't have operating system install gets automtically an IP address by DHCP server from the Domain Controller VM. 
</p>

