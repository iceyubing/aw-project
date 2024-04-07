

```mermaid
graph TD

    F[Micro-frontend]
    style F fill:#0000ff, color:#fff

    A((Seach)) --> B["Home Page"]
    style X fill:#0000ff, color:#fff
    B -->|Contains| X[News]
    style Y fill:#0000ff, color:#fff
    B -->|Contains| Y[Favorites]

    style C fill:#0000ff, color:#fff
    B -->|Filter  by store| G[Filtered supermarket page]
    style E fill:#0000ff, color:#fff
    C -->|Contains| H[Product page]
    G -->|Select category| C[Supermarket list]
    B -->|Contains| H
    style D fill:#0000ff, color:#fff    
    B -->|Contains| D[QR scan]

    H -->|Contains| E[Products´ detail （product managment）]
    D -->|Open the scanner| E[Products´ detail （product managment）]
    E -->|Back| B
    
    

  



