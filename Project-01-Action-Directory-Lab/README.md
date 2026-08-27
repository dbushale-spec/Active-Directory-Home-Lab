# Active Directory Home Lab

## Project Goal

To build a realistic Windows Server environment and gain hands-on experience with tasks commonly performed by IT Support and Help Desk professionals.

---

## Skills Demonstrated

- Windows Server Administration
- Active Directory
- User Management
- Security Groups
- Password Resets
- Account Administration
- Group Policy
- Troubleshooting

---

## Technologies Used

- VirtualBox
- Windows Server 2022
- Windows 10
- Active Directory Domain Services

---

## Progress Tracker

- [X] Install VirtualBox
- [X] Download Windows Server 2022
- [X] Create Domain Controller
- [X] Install Active Directory
- [X] Create Organisational Units
- [X] Create Users
- [X] Create Security Groups
- [X] Reset User Passwords
- [X] Disable User Accounts
- [X] Create Windows 10 Client
- [ ] Join Client To Domain
- [ ] Configure Group Policy

---

## Learning Notes  
## Step 1 - VirtualBox Installation
### What I Did
Successfully installed and launched Oracle VirtualBox.
### What I Learned
I learned that virtualization allows me to run multiple operating systems on one physical computer. Oracle VirtualBox will be used throughout this project to build a safe Active Directory lab without affecting my main Windows installation.

## Step 2 - Windows Server 2022 ISO
### What I Did
Downloaded the Windows Server 2022 Evaluation ISO from Microsoft.
### What I Learned
I learned that an ISO file contains the installation media required to install an operating system. I will use this Windows Server 2022 Evaluation ISO inside VirtualBox to build a realistic Active Directory lab environment.

## Step 3 - Windows Server Installation Complete
### What I Did
Successfully installed Windows Server 2022 and verified that the server booted to the Windows desktop.
### What I Learned
I learned how to deploy a Windows Server operating system inside a virtual machine. This server will later be promoted to a Domain Controller and will host Active Directory Domain Services for the lab.

## Step 4 - Server Manager Dashboard
### What I Did
Opened Server Manager after the first login and confirmed the installation completed successfully.
### What I Learned
I learned that Server Manager is the primary management console used to configure Windows Server. It allows administrators to install server roles and features, monitor the server, and manage services such as Active Directory.

## Step 5 - Rename Server to DC01
### What I Did
Renamed the Windows Server computer name from the default hostname to **DC01** and verified the change in Server Manager.
### What I Learned
I learned that using a descriptive server name makes administration easier and helps identify the server's role within the network. Naming the server DC01 prepares it for its role as the Domain Controller.

## Step 6 - Create Domain Controller
### What I Did
Installed Active Directory Domain Services (AD DS), promoted the server to a Domain Controller, created a new forest named company.local, and verified that DC01 appeared in the Domain Controllers container within Active Directory Users and Computers.
### What I Learned
I learned that a Domain Controller stores and manages Active Directory data, authenticates users and computers, and provides centralized administration for a Windows domain. Promoting the server to a Domain Controller created the company.local domain and prepared the environment for user, group, and policy management.

## Step 7 - Create Organizational Units
### What I Did
Created Organizational Units named Employees, IT, HR, and Finance within Active Directory Users and Computers.
### What I Learned
I learned that Organizational Units (OUs) are used to logically organize Active Directory objects. OUs allow administrators to group users and computers by department and simplify management, delegation, and Group Policy deployment.

## Step 8 - Create Users 
### What I Did
Created user accounts within the IT, HR, and Finance Organizational Units and verified that each account appeared correctly in Active Directory Users and Computers.
### What I Learned
I learned that user accounts can be organized within Organizational Units (OUs) to reflect departmental structures. This makes user administration easier and allows administrators to apply permissions, policies, and management tasks to specific groups of users.

## Step 9 - Create Security Groups
### What I Did
Created security groups named **IT_Users**, **HR_Users**, and **Finance_Users** within Active Directory Users and Computers. Added the appropriate departmental user accounts to each group and verified that the memberships were configured correctly.
### What I Learned
I learned that Security Groups are used to simplify permission management in Active Directory. Instead of assigning permissions to individual users, administrators can assign permissions to groups, making access control easier to manage and maintain.

## Step 10 - Reset User Passwords
### What I Did
Reset passwords for user accounts in the Finance, HR, and IT Organizational Units using Active Directory Users and Computers. Verified that each password reset was completed successfully for the selected user accounts.
### What I Learned
I learned how to reset user passwords in Active Directory and manage user credentials within a domain environment. This task demonstrated how administrators can assist users who forget their passwords while maintaining account security and ensuring continued access to network resources.

# Step 11 - Disable User Accounts
### What I Did
I disabled a user account in each department Organizational Unit (Finance, HR, and IT) using Active Directory Users and Computers. I selected a user from each department and used the Disable Account option to prevent access to domain resources.
### What I Learned
I learned how to disable Active Directory user accounts without deleting them. Disabling accounts is useful when access needs to be temporarily revoked while preserving user information and permissions.

# Step 12 – Create Windows 10 Client
## What I Did
I installed Windows 10 on the Client Virtual Machine using the Windows 10 ISO file in Oracle VirtualBox. During the installation process, I configured the regional settings, selected the Windows edition, accepted the licence agreement, chose the installation type, selected the virtual hard disk, and initiated the operating system installation.
## What I Learned
I learned how to deploy a Windows 10 operating system within a virtualised environment using Oracle VirtualBox. I gained practical experience with the Windows Setup wizard, operating system selection, storage configuration, and the installation stages required to prepare a client machine for use within an Active Directory environment.


---

## Screenshots / Evidence
### Step 1 - VirtualBox Successfully Installed
Oracle VirtualBox was successfully installed and is ready to host the Windows Server virtual machine.
![VirtualBox Successfully Installed](01-virtualbox-installed.png)

### Step 2 - Windows Server 2022 ISO Downloaded
The Windows Server 2022 Evaluation ISO was downloaded successfully from Microsoft.
![Windows Server 2022 ISO Downloaded](02-windows-server-2022-iso.png)

### Step 3 - Windows Server Installation Complete
Windows Server 2022 installation completed successfully, and the server booted to the desktop.
![Windows Server Desktop](03-windows-server-desktop.png)

### Step 4 - Server Manager Dashboard
Server Manager opened automatically after the first login, confirming the installation was successful.
![Server Manager Dashboard](04-server-manager-dashboard.png)

### Step 5 - Server Renamed to DC01
The Windows Server computer name was successfully renamed to DC01 and verified in Server Manager.
![Server Renamed to DC01](05-server-renamed-dc01.png)

### Step 6 - Domain Controller Created
Active Directory Domain Services (AD DS) was installed and the server was successfully promoted to a Domain Controller. The new domain `company.local` was created and DC01 was verified in the Domain Controllers container.
![Domain Controller Created](06-domain-controller-created.png)

### Step 7 - Organizational Units Created
Organizational Units were created to organize users and computers by department. This structure makes administration and Group Policy management easier.
![Organizational Units Created](07-organizational-units-created.png)

### Step 8 - Users created in Organizational Units
#### Step 8.1 - IT Users Created
Successfully created and verified IT user accounts within Active Directory Users and Computers.
![IT Users](08-IT-users.png)
#### Step 8.2 - HR Users Created
Successfully created and verified HR user accounts within Active Directory Users and Computers.
![HR Users](08-HR-users.png)
#### Step 8.3 - Finance Users Created
Successfully created and verified Finance user accounts within Active Directory Users and Computers.
![Finance Users](08-Finance-users.png)

## Step 9 - Security Groups Created
### Step 9.1 - IT Security Group Created
Successfully created the **IT_Users** security group and verified that IT department user accounts were added as members.
![IT Security Group Created](09-IT-security-group.png)
### Step 9.2 - HR Security Group Created
Successfully created the **HR_Users** security group and verified that HR department user accounts were added as members.
![HR Security Group Created](09-HR-security-group.png)
### Step 9.3 - Finance Security Group Created
Successfully created the **Finance_Users** security group and verified that Finance department user accounts were added as members.
![Finance Security Group Created](09-Finance-security-group.png)

## Step 10 - User Passwords Reset
### Step 10.1 - Finance User Password Reset
Successfully reset the password for the Finance department user account using Active Directory Users and Computers.
![Finance User Password Reset](10-finance-password-reset.png)
### Step 10.2 - HR User Password Reset
Successfully reset the password for the HR department user account and verified that the password change was applied successfully.
![HR User Password Reset](10-hr-password-reset.png)
### Step 10.3 - IT User Password Reset
Successfully reset the password for the IT department user account and confirmed the operation completed successfully.
![IT User Password Reset](10-it-password-reset.png)

## Step 11 - Disable User Accounts
### Step 11.1 - Finance User Account Disabled
The screenshot below shows a Finance department user account that has been successfully disabled in Active Directory Users and Computers.
![Finance User Account Disabled](11-finance-user-disabled.png)
### Step 11.2 - HR User Account Disabled
The screenshot below shows an HR department user account that has been successfully disabled in Active Directory Users and Computers.
![HR User Account Disabled](11-hr-user-disabled.png)
### Step 11.3 - IT User Account Disabled
The screenshot below shows an IT department user account that has been successfully disabled in Active Directory Users and Computers.
![IT User Account Disabled](11-it-user-disabled.png)

## Step 12 – Create Windows 10 Client
### Step 12.1 – Launch Windows Setup
The screenshot below shows the Windows Setup wizard successfully loading after booting from the Windows 10 installation ISO.
![Launch Windows Setup](Step%2012.1%20-%20Launch%20Windows%20Setup.png)
### Step 12.2 – Configure Language and Regional Settings
The screenshot below shows the language, time and currency format, and keyboard input settings configured before beginning the Windows installation.
![Configure Language and Regional Settings](Step%2012.2%20-%20Configure%20Language%20and%20Regional%20Settings.png)
### Step 12.3 – Start Windows Installation
The screenshot below shows the Windows Setup screen where the **Install Now** option was selected to begin the Windows 10 installation process.
![Start Windows Installation](Step%2012.3%20-%20Start%20Windows%20Installation.png)
### Step 12.4 – Select Windows Edition
The screenshot below shows the Windows edition selection screen where the required version of Windows 10 was chosen for installation.
![Select Windows Edition](Step%2012.4%20-%20Select%20Windows%20Edition.png)
### Step 12.5 – Accept Microsoft License Terms
The screenshot below shows the Microsoft Software License Terms page where the licence agreement was accepted before continuing the installation.
![Accept Microsoft License Terms](Step%2012.5%20-%20Accept%20Microsoft%20License%20Terms.png)
### Step 12.6 – Choose Installation Type and Target Drive
The screenshot below shows the installation configuration screen where the virtual hard disk was selected as the destination for the Windows 10 installation.
![Choose Installation Type and Target Drive](Step%2012.6%20-%20Choose%20Installation%20Type%20and%20Target%20Drive.png)
### Step 12.7 – Install Windows 10
The screenshot below shows Windows Setup actively installing the operating system onto the virtual hard disk.
![Install Windows 10](Step%2012.7%20-%20Install%20Windows%2010.png)


