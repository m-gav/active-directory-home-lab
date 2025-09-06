```mermaid
flowchart TD
  DC[Server2025 DomainController ADDS DNS GPO]

  Admin[AdminClient IT]
  U1[Client1 HR]
  U2[Client2 Management]
  U3[Client3 Finance]

  DC --> Admin
  DC --> U1
  DC --> U2
  DC --> U3
