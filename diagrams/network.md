```mermaid
flowchart TD
  DC[Windows Server 2025 - Domain Controller - AD DS DNS GPO]

  Admin[Admin Client - Helpdesk - IT]
  U1[User Client 1 - HR]
  U2[User Client 2 - Management]
  U3[User Client 3 - Finance]

  DC --> Admin
  DC --> U1
  DC --> U2
  DC --> U3
