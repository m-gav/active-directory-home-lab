```mermaid
graph TD
    DC[🖥️ Windows Server 2025 - Domain Controller\nRoles: AD DS, DNS, GPO]

    Admin[💻 Admin Client (Helpdesk)\nDomain Joined]
    U1[💻 User Client 1\nRegular User\nDomain Joined]
    U2[💻 User Client 2\nRegular User\nDomain Joined]
    U3[💻 User Client 3\nRegular User\nDomain Joined]

    DC --> Admin
    DC --> U1
    DC --> U2
    DC --> U3
