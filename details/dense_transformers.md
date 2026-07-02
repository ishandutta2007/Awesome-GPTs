# Dense Transformers (Traditional Baseline)

Dense transformer architectures form the foundation of early and modern baseline systems.

```mermaid
flowchart LR
    Input[Input Tokens] --> Layer1[Attention & FFN (100% Active)]
    Layer1 --> Layer2[Attention & FFN (100% Active)]
    Layer2 --> Output[Output Probability]
```

### Overview
- **Complete Layer Activation:** Every single forward pass utilizes all parameter weights in the transformer graph, ensuring high fidelity but introducing extreme compute costs at scale.
- **Attention and Feed-Forward Networks:** Leverages Multi-Head Attention coupled with standard dense FFN architectures.

[← Back to README](../README.md)
