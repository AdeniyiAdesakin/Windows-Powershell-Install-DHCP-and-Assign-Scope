<h1>Install DHCP using PowerShell</h1>
<p>1. To install DHCP using Powershell; Open powershell on your server and type the following command; <b><i> “Install-WindowsFeature DHCP -IncludeManagementTools”</i></b> and hit enter. This will take some times to install, just wait for it and you will be showned a Success message and the Feature results of what you installed.</p>
<p align="center"><img src="https://i.imgur.com/UEa5TXc.png" height="50%" width="50%"/>

<p>2. To confirm that DHCP is installed, go to server manager-dashboard, click on Tools and check the list</p>
<p align="center"><img src="https://i.imgur.com/qCBb6R7.png" height="50%" width="50%"/>

<br>
<br>

<h1>Assign DHCP Scope using Powershell</h1>
<p>1. To assign scope in DHCP using Power shell; Open power shell on your server and type in the following command; <b><i> “Add-DhcpServerv4Scope -Name "ABM Scope" -StartRange 192.168.10.225 -EndRange 192.168.10.235 -SubnetMask 255.255.255.0”</i></b>. Where Name parameter = The descriptive name you want to give the scope, Start Range and End Rage = The range between the IP adddresses available for lease to Dhcp clients, and Subnet mask = subnet mask of your IP address. </p>
<p align="center"><img src="https://i.imgur.com/Gjwd7Q6.png" height="50%" width="50%"/>

<p>2. To confirm this, from server manager-dashboard, click on Tools and select DHCP. While on the DHCP, go to left pane and expand DHCP, then expand IPV4 and there you can find the Scope(ABM Scope) we just created using power shell </p>
<p align="center"><img src="https://i.imgur.com/f7fGwNP.png" height="50%" width="50%"/>

<br>



