# Windows Server and Active Directory Lab

A small Windows domain environment built in VirtualBox during my NIELIT Calicut cybersecurity internship.

**Built**
- Windows Server 2022 and Windows 11 virtual machines on a host-only network
- Static IP for the server (192.168.56.10) with the client pointed at it for DNS
- Active Directory Domain Services with a new domain (`mydomain.local`)
- Two domain users (user1, user2)
- Group Policy Objects, including one that disables Control Panel access
- DHCP service on the server, with the Windows 11 client obtaining a lease

**Why it matters for security:** Active Directory, Group Policy and DHCP are the core of most corporate Windows networks, so they are what attackers target and defenders monitor.

## Setup log

---

**<u>1. Create Microsoft Server and Windows 11 VMs on VirtualBox</u>**

# 1. Virtual Machine Setup

• Downloaded and installed Windows Server and Windows 11 on VirtualBox.

<img src="./media/image1.png" style="width:6in;height:2.60526in" />

• Configured both to use Host-only network adapter.

<img src="./media/image1.png" style="width:6in;height:2.82292in" />

# <img src="./media/image2.png" style="width:6.00912in;height:2.79645in" />

# 

# <u>2. Set Static IP on Server and Use Host-only Network</u>

# 2. Static IP Configuration

• Set static IP for Windows Server: 192.168.56.10

<img src="./media/image3.png" style="width:6in;height:3.16883in" />

<img src="./media/image4.png" style="width:6in;height:2.45455in" />

**<u>3. Configure Domain Controller in Your Server</u>**

3\. Domain Configuration (AD DS)

• Installed Active Directory Domain Services (AD DS) on Windows Server.

<img src="./media/image5.png" style="width:6in;height:3.15069in" />

<img src="./media/image6.png" style="width:6in;height:3.20694in" />

MyDomain.local

<img src="./media/image7.png" style="width:6in;height:3.34861in" />

**<u>4. Create Two Domain Users and Group Policies</u>**

6\. Domain Users Creation

<img src="./media/image8.png" style="width:6in;height:3.76623in" />

# 7. Group Policy Objects (GPO)

• Created GPO1 to disable Control Panel access.

• Created GPO2

<img src="./media/image9.png" style="width:6in;height:2.76623in" />

**<u>5. Configure DHCP Service on Server</u>**

**8. Dhcp**

<img src="./media/image10.png" style="width:6in;height:2.51948in" /><img src="./media/image11.png" style="width:6in;height:3.13403in" />

**Conclusion**

All components were successfully configured and tested.

