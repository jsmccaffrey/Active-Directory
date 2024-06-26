# Active-Directory
Setup Basic Home Lab Running Active Directory and Bulk Add Users
- [Oracle VirtualBox and Extension Pack](https://www.virtualbox.org/wiki/Downloads)
- [Windows 10](https://www.microsoft.com/en-us/software-download/windows10)
- [Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019)

1. Download required files
2. Open VirtualBox and create Windows 10 and Server 2019 virtual machines
3. Server 2019 VM will be the Domain Controller (DC):
  - Set up IP Addressing and rename PC
  - Install Active Directory Domain Services and create domain
    - Configure post-deployment such as naming domain and password
    - Create dedicated domain admin account
    - Create organizational unit, new user, and make domain admin
  - Set up routing and remote access
    - Install NAT
    - Configure DHCP Server
4. Run PowerShell Script to bulk add users
  - Inside the Domain Controller, run the PowerShell Script
  - Creates users with account password, given name, surname, and user ID
  - Uses names from text file and with a default password
5. Windows 10 VM will act as client:
  - Configure user
  - Add Domain Controller
  - Set up Address Lease for computer
  - Active Directory users can now use their account details to log in

![image](https://github.com/jsmccaffrey/Active-Directory/assets/84482329/3ec0bf26-90e5-45db-9283-d762e4064288)
![image](https://github.com/jsmccaffrey/Active-Directory/assets/84482329/b49c7523-612b-4c8e-919e-086c4e922e35)
![image](https://github.com/jsmccaffrey/Active-Directory/assets/84482329/489fac95-f891-47a2-bde7-0aea1425879c)





