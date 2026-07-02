# Sparsely Routed Mixture-of-Experts (Sparse MoE)

Mixture-of-Experts decouples model capacity from actual inference-time compute.

```mermaid
flowchart TD
    Token[Incoming Token] --> Router[Gating / Routing Network]
    Router -->|Route to Top-k| Expert1[Expert 1]
    Router -->|Route to Top-k| Expert2[Expert 2]
    Router -.-> ExpertN[Expert N]
    Expert1 --> Combine[Combine Outputs]
    Expert2 --> Combine
    Combine --> Next[Next Layer]
```

### Overview
- **Routing Network:** Dynamically directs token embeddings to selected expert feed-forward sub-networks.
- **Sparse Activation:** Active parameter count remains small relative to the total capacity, optimizing scaling efficiency.

[← Back to README](../README.md)
