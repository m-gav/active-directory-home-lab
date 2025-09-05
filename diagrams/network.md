```mermaid
graph TD
    DC[🖥️ Windows Server 2025<br/>(Domain Controller)<br/>Roles: AD DS, DNS, GPO]

    Admin[💻 Admin Client<br/>(Helpdesk)<br/>Domain Joined]
    U1[💻 User Client 1<br/>Regular User<br/>Domain Joined]
    U2[💻 User Client 2<br/>Regular User<br/>Domain Joined]
    U3[💻 User Client 3<br/>Regular User<br/>Domain Joined]

    DC --> Admin
    DC --> U1
    DC --> U2
    DC --> U3
