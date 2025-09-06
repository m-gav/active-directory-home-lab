```mermaid
flowchart TD
  DC["Windows Server 2025 - Domain Controller AD DS DNS GPO"]
  Admin["Admin Client - Helpdesk - IT]
  U1["User Client 1 - Regular User - HR"]
  U2["User Client 2 - Regular User - Management"]
  U3["User Client 3 - Regular User - Finance"]

  DC --> Admin
  DC --> U1
  DC --> U2
  DC --> U3
