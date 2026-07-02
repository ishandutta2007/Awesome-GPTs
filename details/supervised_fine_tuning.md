# Supervised Fine-Tuning (SFT) Alignment

Supervised fine-tuning guides raw base models to match target response formats.

```mermaid
flowchart LR
    Base[Pre-trained Model] --> SFT[Train on High-Quality Instruction Pairs]
    SFT --> Aligned[SFT Aligned Model]
```

### Overview
- **Instruction Data:** Involves training the model on clean, manually-curated prompt-response pairs.
- **Formatting Guidance:** Conditions parameters to behave like an assistant, adopting structure, helpfulness guidelines, and formatting standards.

[← Back to README](../README.md)
