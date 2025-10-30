<p align="center">
  <img src="https://raw.githubusercontent.com/tylergehm/vpn-setup/main/vpn.png" alt="GitHub banner" style="max-width:100%;height:auto;" />
</p>
<h1>VPN Setup and Usage within Microsoft Azure Virtual Machines</h1>
A VPN, or Virtual Private Network, is a technology that creates a secure, encrypted connection over the internet between your device and a remote server, allowing you to browse the web privately and securely. By routing your internet traffic through this server, a VPN masks your IP address, making it appear as though you're accessing the internet from a different location, which helps protect your online privacy and bypass geo-restrictions. It's commonly used to safeguard data on public Wi-Fi, access region-locked content, or maintain anonymity online, though it doesn't make you completely untraceable and relies on the trustworthiness of the VPN provider.
</p>


<h2>Environments and Technologies Used</h2>

- Proton VPN (Virtual Private Network)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Website: https://whatismyipaddress.com/

<h2>Operating Systems Used </h2>
- Windows 11 Home (Host Machine)</p>
- Windows 11 Pro </b> (Virtual Machine)

<h2>Steps Included</h2>

- Step 1 - Identifying local IP Address
- Step 2 - Installing Proton VPN
- Step 3 - Configuring Proton VPN
- Step 4 - Identifying new Local IP Address
  
<h2>- Step 1 - Identifying local IP Address </h2>

<img width="1230" height="323" alt="image" src="https://github.com/user-attachments/assets/2de933fe-b241-4653-a09d-1c7d636146d9" />
Note: This demonstration uses a Virtual Machine created in a previous project:  [Creating Virtual Machines in Azure Portal](https://github.com/tylergehm/vm)
</p>
Observing the details of the VM, the Public IP Address is 172.206.17.5 and the VM is being hosted in Microsoft Azure's East US 2 server.
</p>

