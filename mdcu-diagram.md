# MDCU Mermaid Diagram

This file contains a Mermaid flowchart that visualizes the Matt Damon Cinematic Universe. Paste this into any Mermaid-capable Markdown viewer (including GitHub) to render the diagram.

```mermaid
flowchart LR

    %% ====== ERA CLUSTERS ======
    subgraph Origin_&_Early_Life
        CUF[Courage Under Fire
Spec. Ilario
(Gulf War — origin)]
        RAIN[The Rainmaker
Rudy Baylor
(Memphis legal crusader)]
        GWH[Good Will Hunting
Will Hunting
(Boston prodigy)]
        ROUND[Rounders
Mike McDermott
(NYC underground poker)]
        O1[Ocean's Eleven
Linus Caldwell]
        O2[Ocean's Twelve
Linus Caldwell]
        O3[Ocean's Thirteen
Linus Caldwell]
    end

    subgraph Military_&_Black_Ops
        GZ[Green Zone
Roy Miller
(Iraq — WMD investigator)]
        B1[Bourne Identity
Jason Bourne / David Webb]
        B2[Bourne Supremacy]
        B3[Bourne Ultimatum]
        JB[Jason Bourne (2016)]
        DEP[The Departed
Colin Sullivan]
        CUT[The Rip
alias classified]
        INF[The Informant!
Mark Whitacre]
    end

    subgraph Corporate_&_Political
        SYR[Syriana
Bryan Woodman]
        STILL[Stillwater
Bill Baker]
        TAB[The Adjustment Bureau
David Norris]
        PROM[Promised Land
Steve Butler]
        CON[Contagion
Mitch Emhoff]
    end

    subgraph Spacefaring_Era
        MAR[The Martian
Mark Watney]
        INT[Interstellar
Dr. Mann]
    end

    subgraph Authored_Works
        TGW[The Great Wall
William Garin]
        SPR[Saving Private Ryan
Pvt. James Ryan]
        RIP[The Talented Mr. Ripley
Tom Ripley]
        DOG[Dogma
Loki]
        GSHEP[The Good Shepherd
Edward Wilson]
        TGRIT[True Grit
LaBoeuf]
        MMEN[The Monuments Men
James Granger]
        SUY[Stuck on You
Bob Tenor]
        TLD[The Last Duel
Jean de Carrouges]
        THOR[Thor: Love and Thunder
Asgardian actor]
    end

    subgraph Far_Future
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
    CUF --> RAIN --> GWH --> ROUND --> O1 --> O2 --> O3 --> GZ --> B1 --> B2 --> B3 --> JB
    JB --> DEP --> CUT --> INF --> SYR --> STILL --> TAB --> PROM --> CON --> MAR --> INT --> ELY

    %% ====== AUTHORED WORKS (WRITTEN DURING INTERSTELLAR ISOLATION) ======
    INT -.wrote while stranded/.-> TGW
    INT -.wrote while stranded/.-> SPR
    INT -.wrote while stranded/.-> RIP
    INT -.wrote while stranded/.-> DOG
    INT -.wrote while stranded/.-> GSHEP
    INT -.wrote while stranded/.-> TGRIT
    INT -.wrote while stranded/.-> MMEN
    INT -.wrote while stranded/.-> SUY
    INT -.wrote while stranded/.-> TLD
    INT -.wrote while stranded/.-> THOR

    %% ====== META-FORCES CONNECTIONS ======
    AB --- TAB
    AB -.subtle nudges/.-> CUF
    AB -.subtle nudges/.-> RAIN
    AB -.recruitment influence/.-> B1

    BULK --- INT
    BULK -.timeline re-threading/.-> TGW
    BULK -.preserves consciousness/.-> ELY

    %% ====== STYLING ======
    classDef core fill:#f5f5f5,stroke:#333,stroke-width:1px;
    classDef meta fill:#e0f7fa,stroke:#006064,stroke-width:1px;
    classDef sim  fill:#fff8e1,stroke:#f9a825,stroke-width:1px;
    classDef authored fill:#1e1535,stroke:#7c3aed,stroke-width:1px,color:#c4b5fd;
    class CUF,RAIN,GWH,ROUND,O1,O2,O3,GZ,B1,B2,B3,JB,DEP,CUT,INF,SYR,TAB,CON,MAR,INT,ELY core;
    class AB,BULK meta;
    class TGW,SPR,RIP,DOG,GSHEP,TGRIT,MMEN,SUY,TLD,THOR authored;
```
