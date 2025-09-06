```mermaid
flowchart TB
  subgraph Network["VirtualBox Internal Network"]
      A --> B
      P1[" "]  %% invisible node with a single space
  end
  style P1 fill:none,stroke:none

  DC[Windows Server 2025 - Domain Controller - AD DS DNS GPO]

  %% OUs
  subgraph OU_IT["OU: IT"]
      P_IT[ ]  %% padding
      Admin[Admin Client - Helpdesk]
      style P_IT fill:none,stroke:none
  end

  subgraph OU_HR["OU: HR"]
      P_HR[ ]  %% padding
      U1[User Client 1]
      style P_HR fill:none,stroke:none
  end

  subgraph OU_Management["OU: Management"]
      P_MGMT[ ]  %% padding
      U2[User Client 2]
      style P_MGMT fill:none,stroke:none
  end

  subgraph OU_Finance["OU: Finance"]
      P_FIN[ ]  %% padding
      U3[User Client 3]
      style P_FIN fill:none,stroke:none
  end

  %% Connections
  DC --> Admin
  DC --> U1
  DC --> U2
  DC --> U3
