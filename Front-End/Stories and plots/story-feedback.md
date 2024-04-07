```mermaid
graph TD

    F[Micro-frontend]
    style F fill:#0000ff, color:#fff

    A((Feedback)) --> B["Home Page"]
    style X fill:#0000ff, color:#fff
    B -->|Contains| X[News]
    style Y fill:#0000ff, color:#fff
    B -->|Contains| Y[Favorites]
    style Z fill:#0000ff, color:#fff
    B -->|Contains| Z[QR scanner]


    style C fill:#0000ff, color:#fff
    B -->|Filter  by store| G[Filtered supermarket page]
    style E fill:#0000ff, color:#fff
    C -->|Contains| H[Products page]
    G -->|Select category| C[Supermarket list]
    B -->|Contains| H[Product page]
    

    H -->|Contains| E[Products´ detail （product managment）]
    
    H -->|Select  product and give feedback| I[Feedback page]
    style J fill:#0000ff, color:#fff 
    I -->|contains| J[Feedback]
    J -->|Giving a star rating| I
    I -->|Back| H
    


