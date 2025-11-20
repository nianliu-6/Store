# Kernel Comparison of CNN Architectures

```mermaid
graph TD;
    A[Traditional Small Kernel Stacking CNN] -->|Stacked Convolutions| B[Feature Extraction]
    A -->|Reduce Parameters| C[Efficiency]
    A -->|Better Local Features| D[Small Object Recognition]

    E[Large Kernel Design Paradigm (UniRepLKNet)] -->|Single Large Convolution| F[Global Context]
    E -->|Fewer Layers| G[Reduced Complexity]
    E -->|Captures Large Features| H[Large Object Recognition]

    style A fill:#f9f,stroke:#333,stroke-width:2px;
    style E fill:#bbf,stroke:#333,stroke-width:2px;
```
