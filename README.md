# Vitual Private Network (VPN)
<p align="center">
<img src="https://github.com/user-attachments/assets/148ea37f-12b6-4db2-9a6d-dd2d9df49395" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>VPN - Setup and Usuage</h1>
In this project we will set up a Virtual Private Network (VPN) by first creating a Virtual Machine in Microsoft Azure. From there we will configure the necessary network settings to establish secure remote connections within a network infrastructure.<br />

<h2>Environments and Technologies Used</h2>

- Proton VPN (Virtual Private Network)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 11 </b> (24H2)

<h2>Steps Included</h2>

- STEP 1 - Locating our local IP address
- STEP 2 - Setting up a Virtual Machine in Microsoft Azure
- STEP 3 - Locating our IP address through the Virtual Machine (France)
- STEP 4 - Connecting to Proton VPN (Virtual Private Network) courtesy of the Virtual Machine
- STEP 5 - Locating our IP address through the VPN (Netherlands)

<h2>Installation Steps</h2>

STEP 1 - We began this exercise by going to "www.whatismyipaddress.com" to find our local IP address. Use EXAMPLE 1A below as a reference guide.

EXAMPLE 1A
<p>
<img <img width="1820" height="809" alt="VPN 1" src="https://github.com/user-attachments/assets/5b352c4b-9f75-45bd-8699-30956443324e" />

</p>
<p>

Now that our local IP address was found the next thing to do is set up our Virtual Machine in Microsoft Azure. 
  
</p>
<br />

STEP 2 - In order to create a Virtual Machine, we must first create a Resource Group. After the Resource Group has been created type Virtual Machines into the search bar. Click on "Create" followed by the Virtual Machine tab to began creating one like we've done in EXAMPLE 2A. 

EXAMPLE 2A
<p>
<img <img width="1653" height="773" alt="VPN 2" src="https://github.com/user-attachments/assets/9b1eb6f1-78f4-4900-b438-2a88e1a10a79" />

</p>
<p>

Be sure to select the name you used when you created the Resource Group under the firt section Project details - Subscription* - Resource group* (in ours "VPN-Test" is the name). DO NOT create a new Resource Group name. Enter a Virtual machine name (we chose “FranceVM” as the name). Ensure that the other items are checked as shown in EXAMPLES 2B & 2C.

EXAMPLE 2B
<p>
<img <img width="1064" height="710" alt="VPN 3" src="https://github.com/user-attachments/assets/a835454e-0eb7-42e0-bbc6-02e604544308" />

</p>
<p>

NOTE: for the Username and Password we created our own credentials (as shown in EXAMPLE 2C).
  
</p>
<br />

EXAMPLE 2C
<p>
<img <img width="935" height="694" alt="VPN 4" src="https://github.com/user-attachments/assets/db6a4961-269d-42e3-b8eb-ac29f4ef68fa" />

</p>
<p>

Select the tab that says "Networking" (Basics -> Disks -> Networking) towards the top of the page and view EXAMPLE 2D to ensure the inputs match. 
  
</p>
<br />

EXAMPLE 2D
<p>
<img <img width="1029" height="822" alt="VPN 5" src="https://github.com/user-attachments/assets/978161fc-9de6-43b7-a7ea-b520ff2cadc1" />

</p>
<p>

Select “Review and Create” and wait a few seconds for it to pass validation. After it passes validation select “Create” at the bottom. You will receive a follow-up notification that says "deployment in progress" so be prepared to wait for about 2-3 minutes for it to complete the deployment.
  
</p>
<br />

Once deployment is finished we can click on our Virtual Machine to open it. There we will discover our Virtual Machine's Public IP address and other information as shown below in EXAMPLE 2E.

EXAMPLE 2E

<p>
<img <img width="1661" height="783" alt="VPN 6" src="https://github.com/user-attachments/assets/edca9eb6-e2d6-485c-9507-982c80dc8f6f" />

</p>
<p>


STEP 3 – Log into the Virtual Machine and find the IP address
<p>
Since we have set up our Virtual Machine we can connect to it using Remote Desktop (see EXAMPLE 3A below). Input the IP address our Virtual Machine generated (scroll back up to EXAMPLE 2E for help) as the Computer and then type in the Username + Password (scroll back up to EXAMPLE 2C for help). After successfully logging into Remote Desktop, open the web browser and type in www.whatismyipaddress.com as shown below in EXAMPLE 3B.

  
</p>
<br />
EXAMPLE 3A
<p>
<img <img width="599" height="371" alt="VPN 7" src="https://github.com/user-attachments/assets/38946338-4184-4359-92f9-49bd763123ea" />

</p>
<p>

  
</p>
<br />

EXAMPLE 3B
<p>
<img <img width="1799" height="682" alt="VPN 8" src="https://github.com/user-attachments/assets/26221819-21df-4349-8b82-52804cb097aa" />

</p>
<p>

When we look up the IP address for the Virtual Machine through www.whatismyipaddress.com we now see it's showing Amazon.com as our Internet Service Provider (ISP) and our location has now changed to France (see EXAMPLE 3C).
  
</p>
<br />

EXAMPLE 3C
<p>
<img <img width="1799" height="682" alt="VPN 8" src="https://github.com/user-attachments/assets/95a8852b-8e39-4e9b-87d8-b4d4117bfc01" />

</p>
<p>

STEP 4 – Connecting to the VPN (Free Version)

Using our local computer (not Remote Desktop) head to www.protonvpn.com and create a free account. DO NOT use the Virtual Machine because French will be displayed on the browser since our location has changed to France (as mentioned in EXAMPLE 3C). After logging into our account, let's copy the URL from Proton VPN's website (see EXAMPLE 4A) & paste it into to our VM's web browser. 

  
</p>
<br />

EXAMPLE 4A
<p>
<img <img width="1408" height="937" alt="VPN 10" src="https://github.com/user-attachments/assets/98ae99f3-3bb0-49fb-9506-35fbe010a5a8" />

</p>
<p>

Now scroll down the and select the “Downloads" tab. Here we can choose which operating system we want to download the VPN on. In our case we selected Windows (as shown in EXAMPLE 4B). Once the download completes the application is now installed.  
  
</p>
<br />


EXAMPLE 4B
<p>
<img <img width="1625" height="944" alt="VPN 11" src="https://github.com/user-attachments/assets/f0621ae7-378e-4438-81bc-15ad52799e18" />

</p>
<p>

Open the app and log in using the credentials we created for the free account. Click on Connect to began finding a server. EXAMPLE 4C below shows that the Netherlands was selected as the fastest free server for our connection.
  
</p>
<br />

EXAMPLE 4C
<p>
<img <img width="1713" height="966" alt="VPN 12" src="https://github.com/user-attachments/assets/30bac208-db22-45aa-8216-d4f52477df45" />

</p>
<p>

Using our VM browser, we will look up our IP address one last time now that the VPN is connected. In EXAMPLE 4D the website www.whatismyipaddress.com shows yet another IP address change using the VPN from the Netherlands. I must say this is quite fascinating!!
  
</p>
<br />

EXAMPLE 4D
<p>
<img width="1708" height="745" alt="VPN 13" src="https://github.com/user-attachments/assets/b5cedd5f-2ffe-4e68-a7e6-4d63d5a5a450" />


</p>
<p>



<h2>Final Thoughts</h2>
This project strengthened my understanding of VPN architecture by implementing a secure network tunnel within a virtualized environment. It also enhanced my skills in configuring, testing, and troubleshooting secure remote connections. When reviewing this project in totality, notice that 3 different IP addresses were utilized just from our local computer to connect to the internet.
Home/Local IP (USA): 99.47.77.196,
Virtual Machine IP (France): 98.66.162.170,
Virtual Machine IP VPN (Netherlands): 80.79.7.127

  
</p>
<br />
