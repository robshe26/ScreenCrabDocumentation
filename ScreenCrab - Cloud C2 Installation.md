# Cloud C2 Installation Guide

This is a guide on the download and setup of Hak5's Clould C2 software

## Pre-Install Requirements 

- Virtual Box or any Virtual Machine software
- Installation of Windows Server 2022 on the Virtual Machine
- Network adapter to: NAT

## Step 1: Download the software Cloud C2

1. In the Windows Server VM:
- Go to Windows Defender Firewall>Turn Windows Defender Firewall on or off
  - Turn OFF all firewall settings
    
2.
- Go to [Hak5] (https://downloads.hak5.org/cloudc2)

___Example pictured here:___
<img width="975" height="734" alt="image" src="https://github.com/user-attachments/assets/3ea00913-11ce-4685-a3c2-a0d812716c74" />

- Select 3.5.2-stable and download it
    - If the download fails and returns, **Couldn't Download - Virus Detected**, do the following
        - Go to Windows Security>Virus & threat protection>Protection history
        - Find the threat related to the download of the server file
___Example pictured here:___
<img width="799" height="635" alt="image" src="https://github.com/user-attachments/assets/be34310c-bff2-4031-adce-106448b90045" />
          -Go to Actions and click **Allow**
  
4. After the download is complete go to Windows File Manager &rarr; Downloads

___Example pictured here:___
<img width="975" height="678" alt="image" src="https://github.com/user-attachments/assets/e7632eff-d5f8-4fed-b6ac-6336a22f6ff8" />

- Go to the C:\Users\Adminisrtator directory and create a new directory under Adminisrtator for the server
- Click **EXTRACT ALL** on the .zip file in downloads and select your new folder as the destination
- If this was done correclty you should see `c2-3.4.2_amd64_windows.exe` in C:\Users\Adminisrtator\<your_folder_name>
  
___Example pictured here:___
<img width="1022" height="725" alt="image" src="https://github.com/user-attachments/assets/f3edc8a9-ce2e-4610-aa45-bd50ff00a66a" />


5. Start Commnad Prompt(cmd.exe)
- First change the Directory to the Directory with the Server File
- Now start the Cloud C2 server
- c2-3.5.2_amd64_windows.exe -hostname <ip_addr_of_VM>
- After running the previous commmand you should see:
  
___Example pictured here:___
<img width="1021" height="510" alt="image" src="https://github.com/user-attachments/assets/2609f637-f9c8-47ff-8e11-80fd25919418" />

6. Now go to https://www.hakshop.com/products/c2?utm_source=chatgpt.com#c2-versions
- On that page you should see:

___Example pictured here:___
<img width="1157" height="1234" alt="image" src="https://github.com/user-attachments/assets/ba27d186-58d1-43c0-a0ac-a56394fb7c94" />

-Click **Free Download** for the community version
-Complete checkout and have the product key sent one of your emails

7.Now go back to your Virtual Machine
- In the ouput of start the server there should be a Setup Token(you will want to write this down somewhere)
    
___Example pictured here:___
<img width="448" height="358" alt="image" src="https://github.com/user-attachments/assets/762fc77e-f1ab-4bbe-bd72-5d6d5826ec9c" />

- Next connect to the UI of the server through <IP_addr>:8080 in a web browser
    - This should take you to the setup for the server
    ___Example pictured here:___
    <img width="1022" height="733" alt="image" src="https://github.com/user-attachments/assets/48571bc8-2310-43b3-9c28-4da025a2bdc1" />
    - Proceed through the setup using the Token and Product Key
      - Set Username: Lab@<firstInt_LastName>
      - Set Password: Passw0rd!
    - After setup is complete do a First time login to check credentials
  
    ___Example pictured here:___
    <img width="995" height="688" alt="image" src="https://github.com/user-attachments/assets/eb296ac2-c58b-4ab6-99b3-3aa1c99f8d78" />
        - This should be what the UI look like
  
    - Then stop the server, restart it and log in again to make sure everything worked
  




8. Next Setup the Wireless access point
- First take out Asus RT-N66U Dark Knight and plug it into power(NOT THE SWITCH YET)
- Power on the router
- Hold RESET button (back) for 10 seconds, the wait for reboot
- Plug your latop into one of the yellow lan port on the back of the device
- Open a browser and go to http://192.168.1.1
- Log in to the software and go to Adminisration>Operation Mode
- Select: Router Mode -> Save / Apply(Router will reboot)
- Connect to the Router by the browser
- Go to Wireless Settings
- Set SSID: <any_valid_network_name>
           







