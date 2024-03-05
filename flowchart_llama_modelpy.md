``` mermaid

    graph TD
        A[Start] --> B{ModelArgs Data Class}
        B --> C[RMSNorm Class]
        C --> D[Precompute Freqs Function]
        D --> E[Reshape for Broadcast Function]
        E --> F[Apply Rotary Emb Function]
        F --> G[Repeat KV Function]
        G --> H[Attention Class]
        H --> I[Attention Forward Function]
        I --> J[FeedForward Class]
        J --> K[FeedForward Forward Function]
        K --> L[TransformerBlock Class]
        L --> M[TransformerBlock Forward Function]
        M --> N[Transformer Class]
        N --> O[Transformer Forward Function]
        O --> P[End]

        style A fill:#f9f,stroke:#333,stroke-width:4px
        style P fill:#f9f,stroke:#333,stroke-width:4px
```
