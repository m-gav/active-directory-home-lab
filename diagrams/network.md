```mermaid
flowchart TB
  subgraph Network["VirtualBox Internal Network"]

    DC[Windows Server 2025 - Domain Controller - AD DS DNS GPO]

    subgraph OU_IT["OU: IT"]
      Admin[Admin Client - Helpdesk]
    end

    subgraph OU_HR["OU: HR"]
      U1[User Client 1]
    end

    subgraph OU_Management["OU: Management"]
      U2[User Client 2]
    end

    subgraph OU_Finance["OU: Finance"]
      U3[User Client 3]
    end

    DC --> Admin
    DC --> U1
    DC --> U2
    DC --> U3
  end
