# Features

This Active Directory homelab was built using Windows Server 2025 and Windows 11 clients in Oracle VirtualBox.  
It demonstrates my ability to configure, manage, and troubleshoot Active Directory in a real-world environment.  

---

## 🖥Active Directory Domain Services (AD DS)
- Configured Windows Server 2025 as a Domain Controller  
- Installed AD DS and DNS roles  
- Built a domain forest (`homelab.local`)  
- Added multiple domain-joined Windows 11 clients  

![Domain Controller Roles](screenshots/dc-roles.png)  
Figure 1: Server Manager showing AD DS and DNS roles installed

![Domain Tree](screenshots/domain-tree.png)  
Figure 2: Active Directory Users and Computers (ADUC) showing the domain tree

---

##  User and Group Management
- Created users and departmental groups  
- Implemented Organizational Units (OUs) for IT, HR, Management, and Finance  
- Practiced password resets, account lockouts, and group assignments  

![OU Structure](screenshots/ou-structure.png)  
Figure 3: Organizational Units for IT, HR, Management, and Finance

![User Properties](screenshots/user-properties.png)  
Figure 4: User account properties showing group membership and department

![Password Reset](screenshots/reset-password.png)  
Figure 5: Resetting a user password in ADUC

---

## Group Policy Management
- Configured password policy (length, complexity, expiration)  
- Deployed a desktop wallpaper GPO (visual proof of GPO enforcement)  
- Applied login banner for security compliance  
- Disabled Control Panel access for standard users  

![GPO Console](screenshots/gpo-console.png)  
Figure 6: Group Policy Management Console showing applied GPOs

![Wallpaper GPO](screenshots/wallpaper-policy.png)  
Figure 7: Desktop wallpaper enforced via GPO

![Login Banner](screenshots/login-banner.png)  
Figure 8: Security login banner applied via GPO

![Blocked Control Panel](screenshots/blocked-control-panel.png)  
Figure 9: Control Panel access blocked for standard users

---

## DNS & Networking
- Configured DNS zones on the Domain Controller  
- Verified name resolution and connectivity between clients and DC  
- Built a VirtualBox Internal Network for isolation  

![DNS Manager](screenshots/dns-manager.png)  
Figure 10: DNS Manager showing homelab.local zone

![Ping & Nslookup](screenshots/ping-nslookup.png)  
Figure 11: Client successfully resolving DC via DNS

---

## Administration Practice
- Simulated helpdesk tasks: unlocking accounts, resetting passwords, moving users  
- Used a Helpdesk admin account with limited permissions to mimic real-world workflows  

![Helpdesk Login](screenshots/helpdesk-login.png)  
Figure 12: Helpdesk account in Active Directory Users and Computers

![Unlock Account](screenshots/unlock-account.png)  
Figure 13: Unlocking a user account from ADUC

---

## Extensible Design
This homelab can be expanded with:  
- File and Print Services  
- DHCP Server  
- Security monitoring (e.g., SIEM, Splunk, Sysmon)  
- Additional Domain Controllers for redundancy  

![Planned Expansion](screenshots/future-diagram.png)  
Figure 14: Planned extensions such as DHCP, File Server, and Monitoring

---

