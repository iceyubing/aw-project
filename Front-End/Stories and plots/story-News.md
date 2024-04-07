

```mermaid
graph TD

    A[Micro-frontend]
    style A fill:#0000ff, color:#fff
    
    B((News)) --> C[Home Page]
    style Y fill:#0000ff, color:#fff
    C -->|Contains| Y[Favorites]
    style x fill:#0000ff, color:#fff
    C -->|Contains| x[Products management]
    style Z fill:#0000ff, color:#fff
    C -->|Contains| Z[QR scanner]
    C --> |Contains| D[News Page]
    style E fill:#0000ff, color:#fff
    D --> |Check| E[News Management]
    E --> |See more information| F[News details]
    F --> |Back| D 