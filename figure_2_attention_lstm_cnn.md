```mermaid
flowchart LR
    A["Input (network traffic time series)"]:::gray --> B["BorderlineSMOTE preprocessing"]
    B --> C["1D-CNN module (extract local spatial features)"]
    C --> D["BiLSTM module (extract long-distance temporal dependencies)"]
    D --> E["Joint Attention mechanism (with CNN feature assistance)"]:::yellow
    E -->> F["Feature reweighting"]
    F --> G["Fully connected + Softmax"]
    G --> H["Output (normal/attack category)"]:::orange

    classDef gray fill:#C0C0C0;
    classDef yellow fill:#FFFF00;
    classDef orange fill:#FFA500;
```