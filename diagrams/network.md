```mermaid
flowchart TB
  subgraph Network["VirtualBox Internal Network"]

    classDef withmargines fill-opacity:0.0,color:#FFFFFF,stroke-width:0px;
    subgraph foo [<font size = 6>Example of a subgraph that HAS space between name and top node]

        foo1["<p style='width:100px;height:0px;margin:0'>Invisible !!!/p>"]:::withmargines
        box1["Some space above this box and the title"]
        
        foo1 ~~~ box1-->box2
    end

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
