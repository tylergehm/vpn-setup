  <img src="https://raw.githubusercontent.com/tylergehm/vpn-setup/main/vpn.png" alt="GitHub banner" style="max-width:100%;height:auto;" />
</p>
<h1>VPN Setup and Usage within Microsoft Azure Virtual Machines</h1>
A VPN, or Virtual Private Network, is a technology that creates a secure, encrypted connection over the internet between your device and a remote server, allowing you to browse the web privately and securely. By routing your internet traffic through this server, a VPN masks your IP address, making it appear as though you're accessing the internet from a different location, which helps protect your online privacy and bypass geo-restrictions. It's commonly used to safeguard data on public Wi-Fi, access region-locked content, or maintain anonymity online, though it doesn't make you completely untraceable and relies on the trustworthiness of the VPN provider.
</p>
<h2>Video Demonstration</h2>

- ### [YouTube: VPN Setup and Usage within Microsoft Azure Virtual Machines](https://www.youtube.com/watch?v=dcC5xFULLY4)

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
  
<h2>Step 1 - Identifying local IP Address </h2>

<img width="1230" height="323" alt="image" src="https://github.com/user-attachments/assets/2de933fe-b241-4653-a09d-1c7d636146d9" />
Note: This demonstration uses a Virtual Machine created in a previous project:  [Creating Virtual Machines in Azure Portal](https://github.com/tylergehm/vm)
</p>
Observing the details of the VM, the Public IP Address is 172.206.17.5 and the VM is being hosted in Microsoft Azure's East US 2 server.
</p>
<img width="1497" height="755" alt="image" src="https://github.com/user-attachments/assets/291d4da1-f7e0-4b34-9f6c-8d2bde5a1640" />
An alternative way to discover the VM's IP address is to open up an web browser and access the website https://whatismyipaddress.com/. </p>
Here we can see that the website reflects the same IP Address - 172.206.17.5. The website also shows that the IP Address is provided by Microsoft and is located in Boydton, Virginia; which is in the Eastern United States.
</p>

<h2>Step 2 - Installing Proton VPN</h2>
<img width="1886" height="1013" alt="image" src="https://github.com/user-attachments/assets/113fa4ca-089f-4721-aa45-38c7591af519" />
Next, access the website https://protonvpn.com/ to sign up for ProtonVPN and download the software. This will begin by clicking "Get Proton VPN". </p>
Proton VPN is a secure, privacy-focused virtual private network service by Proton that encrypts internet connections and protects user anonymity with a no-logs policy and servers worldwide. 
</p>

<img width="1863" height="918" alt="image" src="https://github.com/user-attachments/assets/925e9620-42d4-46b1-a5f3-30f54fb9516b" />

After clicking "Get Proton VPN", on the next web page, select the "Get Proton Free" option.

</p>

<img width="1287" height="680" alt="image" src="https://github.com/user-attachments/assets/c736a7d9-eac6-46c1-9b52-460884d70898" />

Create an account to sign up with Proton in order to download the Proton VPN.

</p>

<img width="302" height="326" alt="image" src="https://github.com/user-attachments/assets/8ff2d9e1-2ea6-4980-8105-2c7e17702d36" />

Once logged in, click on the "Downloads" section on the left panel of the web page.

</p>

<img width="1232" height="718" alt="image" src="https://github.com/user-attachments/assets/09290c9e-b8bc-40c8-aff2-7e1eda979aea" />

Select Windows Download because the Virtual Machine is running Windows 11 Pro.

</p>


<img width="936" height="601" alt="image" src="https://github.com/user-attachments/assets/f966a1dd-f51c-4131-8511-fa430635d85d" />

Select "Windows 11/10 (x64)". Use the following images as a guide for installation:

</p>

<img width="405" height="211" alt="image" src="https://github.com/user-attachments/assets/706317e9-4047-4c19-bf76-e6cbc2379e15" />

<img width="686" height="563" alt="image" src="https://github.com/user-attachments/assets/4bfd8e21-ea5e-4af6-bf64-d5202c3d90f6" />

<img width="693" height="667" alt="image" src="https://github.com/user-attachments/assets/3bd945dc-e1cc-4601-836e-61579f48456a" />

<img width="1243" height="801" alt="image" src="https://github.com/user-attachments/assets/f8ee5a37-1327-4f93-a595-1d254d9dd0ef" />

<h2>Step 3 - Configuring Proton VPN</h2>

After installation, the program will launch with a Sign-In form. Use the account that was created on the Proton website to sign into Proton VPN.

</p>

<img width="1241" height="725" alt="image" src="https://github.com/user-attachments/assets/18e132a3-89ab-4793-88f0-82784f63402f" />

Once signed in to Proton VPN, click the button that says "Connect". This will begin the process of automatically assigning the computer a new IP address from one of Proton's VPN servers.

</p>
<img width="1238" height="812" alt="image" src="https://github.com/user-attachments/assets/77f46f3e-6bc9-40e1-880b-2b564a6ad267" />

Proton VPN automatically assigned the Windows 11 VM to a server in the Netherlands. 

</p>
<h2>Step 4 - Identifying new Local IP Address</h2>
<img width="1474" height="722" alt="image" src="https://github.com/user-attachments/assets/b0c0075b-aeb1-4f7e-bbdd-79ccf07d69f9" />

Returning to the website https://whatismyipaddress.com/; we can see that the VM has been assigned a new IP Address. </p>
The new IP Address is 89.38.97.198 and is hosted by an Internet Service Provider called WorldStream B.V. The server of the new IP Address is located in Naaldwijk, Netherlands. 

</p>
<img width="1913" height="1018" alt="image" src="https://github.com/user-attachments/assets/0e8dbae5-137e-4925-83fb-b75db4b7d8e7" />
As a secondary test, visiting the website http://www.google.com --- the website is written in Dutch, indicating that this is the Dutch version of Google. 

<h2>Conclusion</h2>
This project successfully demonstrated the setup and usage of Proton VPN within a Microsoft Azure Virtual Machine running Windows 11 Pro, showcasing how a VPN can mask a VM's public IP address to enhance privacy and enable access to region-specific content. By following the steps to identify the initial IP address, install and configure Proton VPN, and verify the new IP address, we confirmed the VPN's ability to reroute traffic through a server in the Netherlands, effectively changing the VM's apparent location from the Eastern United States to Naaldwijk, Netherlands, as evidenced by the updated IP address and access to the Dutch version of Google.
