# MDCU Mermaid Diagram

This file contains a Mermaid flowchart that visualizes the Matt Damon Cinematic Universe. Paste this into any Mermaid-capable Markdown viewer (including GitHub) to render the diagram.

```mermaid
flowchart LR

    %% ====== ERA CLUSTERS ======
    subgraph Early_Legal_&_Boston
        RAIN[The Rainmaker
Rudy Baylor
(early legal crusader)]
        GWH[Good Will Hunting
Will Hunting
(wounded Boston prodigy)]
    end

    subgraph Military_&_Black_Ops
        GZ[Green Zone
Roy Miller
(military crucible)]
        B1[Bourne Identity
Jason Bourne / David Webb]
        B2[Bourne Supremacy]
        B3[Bourne Ultimatum]
        JB[Jason Bourne (2016)]
        DEP[The Departed
Colin Sullivan]
        INF[The Informant!
Mark Whitacre]
    end

    subgraph Corporate_&_Political
        SYR[Syriana
Bryan Woodman]
        TAB[The Adjustment Bureau
David Norris]
        CON[Contagion
Mitch Emhoff]
    end

    subgraph Spacefaring_Era
        MAR[The Martian
Mark Watney]
        INT[Interstellar
Dr. Mann]
    end

    subgraph Far_Future
        TGW[The Great Wall
William Garin
(simulation/mythic run)]
        ELY[Elysium
Max Da Costa]
    end

    subgraph Meta_Forces
        AB[Adjustment Bureau
Plan Editors]
        BULK[Interstellar bulk beings
5D timeline architects]
    end

    %% ====== CORE LIFE PROGRESSION (MOSTLY LINEAR) ======
    RAIN --> GWH --> GZ --> B1 --> B2 --> B3 --> JB
    JB --> DEP --> INF --> SYR --> TAB --> CON --> MAR --> INT --> ELY

    %% ====== SIMULATION BRANCH (NO LITERAL PAST TRAVEL) ======
    INT -.far-future training/.-> TGW
    TGW -.returns to main thread/.-> ELY

    %% ====== META-FORCES CONNECTIONS ======
    AB --- TAB
    AB -.subtle nudges/.-> RAIN
    AB -.recruitment influence/.-> B1

    BULK --- INT
    BULK -.timeline re-threading/.-> TGW
    BULK -.preserves consciousness/.-> ELY

    %% ====== STYLING ======
    classDef core fill:#f5f5f5,stroke:#333,stroke-width:1px;
    classDef meta fill:#e0f7fa,stroke:#006064,stroke-width:1px;
    class RAIN,GWH,GZ,B1,B2,B3,JB,DEP,INF,SYR,TAB,CON,MAR,INT,TGW,ELY core;
    class AB,BULK meta;
```
