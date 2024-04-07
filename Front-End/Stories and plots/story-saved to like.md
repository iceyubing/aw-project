```mermaid
graph TD

    F[Micro-frontend]
    style F fill:#0000ff, color:#fff

    A((Saved to like)) --> B["Home Page"]
    style X fill:#0000ff, color:#fff
    B -->|Contains| X[News]

    style C fill:#0000ff, color:#fff
    B -->|Filter  by store| G[Filtered supermarket page]
    style E fill:#0000ff, color:#fff
    C -->|Contains| H[Product page]
    G -->|Select category| C[Supermarket list]
    B -->|Contains| H
    style D fill:#0000ff, color:#fff    
    B -->|Open the scanner| D[QR scan]

    H -->|Contains| E[Products´ detail （product managment）]
    D -->|Contains| E[Products´ detail （product managment）]
    E -->|Back| B
    style I fill:#0000ff, color:#fff
    E -->|Add to favorites| I["Favorites System"]
    B -->|Contains| J["Favorites Page"]
    J -->|Contains| I["Favorites System"]
    I -->|Remove meat from favorites| I["Favorites System"]

    

