```mermaid
graph TD
    DC[Windows Server 2025 - Domain Controller (AD DS, DNS, GPO)]

    Admin[Admin Client - Helpdesk - Domain Joined]
    U1[User Client 1 - Regular User - Domain Joined]
    U2[User Client 2 - Regular User - Domain Joined]
    U3[User Client 3 - Regular User - Domain Joined]

    DC --> Admin
    DC --> U1
    DC --> U2
    DC --> U3
