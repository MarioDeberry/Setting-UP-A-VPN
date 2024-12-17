# Virtual Private Network (VPN) Setup and Configuration  
![VM Setup Page](https://imgur.com/xrrqQad.png)    

This guide demonstrates how to configure a Virtual Private Network (VPN) using a Virtual Machine (VM) in Microsoft Azure and Proton VPN.  

---

## Prerequisites and Technologies  

### Environments and Tools  
- **VPN Service:** Proton VPN (Free version)  
- **Cloud Platform:** Microsoft Azure  
- **Remote Access:** Remote Desktop  
- **Web Server:** Internet Information Services (IIS)  

### Operating System  
- **Windows 10** (Version 21H2)  

---

## Steps Overview  

1. **Locate Local IP Address**  
2. **Set Up a Virtual Machine (VM) in Azure**  
3. **Find VM IP Address (France)**  
4. **Connect VM to Proton VPN**  
5. **Verify VPN IP Address (Japan)**  

---

## Installation Steps  

### Step 1: Locate Local IP Address  
- Open a browser and navigate to [www.whatismyipaddress.com](https://www.whatismyipaddress.com) to find your local IP address.  
- Save this information for later use.  

  
![Local IP Example](https://imgur.com/nyr29IM.png)  

---

### Step 2: Create a Virtual Machine (VM) in Azure  
- Go to [Azure Portal](https://portal.azure.com) and select **Virtual Machines**.  
  - Create a free account if necessary (Azure offers $200 in free credits).  
- Set the following configurations:  
  - **VM Name:** VM-CanadaCentral  
  - **Region:** Canada Central  
  - **Username/Password:** Create custom credentials and store them securely.  

![VM Configuration](https://imgur.com/oZH8udu.png)
![Networking Tab](https://imgur.com/4xwTr5R.png)


- Select **Review and Create**, and once validation passes, click **Create**.  
- After deployment, note the VM's public IP address (e.g., `4.204.49.129`).  

 
![VM IP Address](https://imgur.com/cEgJ6pI.png)  

---

### Step 3: Log Into the VM and Locate Its IP Address  
- Open **Remote Desktop Connection** on your local computer.  
- Enter the VM's IP address and credentials to log in.  

 
![Remote Desktop App](https://imgur.com/eYn8yN6.png)    

- Inside the VM, use a browser to visit [www.whatismyipaddress.com](https://www.whatismyipaddress.com) and confirm the IP location is in **Canada**.  

 
![VM IP Address France](https://imgur.com/lGylcx3.png)  

---

### Step 4: Connect to Proton VPN in the VM  
- On your local machine, visit [Proton VPN](https://protonvpn.com) and create a free account.  
- Copy the Proton VPN URL and open it in the VM browser.  
- Download and install the Proton VPN application for Windows.  
- Log in with your Proton VPN credentials and connect to the VPN.  

 
![Proton VPN Website](https://i.imgur.com/orO2O5y.png)  
![Proton VPN App Connected](https://imgur.com/jgHr1xX.png)  

- Select a country (e.g., USA ) to connect through the VPN.  

  
![VPN Connected to USA](https://imgur.com/8hv9Czy.png)  

---

### Step 5: Verify VPN IP Address  
- Open a browser in the VM and revisit [www.whatismyipaddress.com](https://www.whatismyipaddress.com).  
- Confirm the IP address now reflects the VPN connection (e.g., **USA**).  

  
![VPN IP Address Japan](https://imgur.com/FEti06X.png)  

---

## Summary  

This process demonstrates how to use multiple IP addresses for secure internet access:  
1. **Local IP (USA):** e.g., `146.70.195.180`  
2. **VM IP (Canada):** e.g., `4.204.49.129`  
3. **VPN IP (USA):** e.g., `149.40.62.18`  


