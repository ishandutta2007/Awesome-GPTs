# Reinforcement Learning with Verifiable Rewards (RLVR)

Replacing subjective reward models with programmatically verifiable loops.

```mermaid
flowchart LR
    Policy[Model Policy] --> Output[Code / Math Output]
    Output --> Verifier[Programmatic Sandbox / Compiler / Equation Solver]
    Verifier -->|Correct / Valid| PosReward[Positive Reward]
    Verifier -->|Incorrect| ZeroReward[Zero / Negative Reward]
    PosReward & ZeroReward -->|Update Policy| Policy
```

### Overview
- **Programmatic Verifiers:** Evaluates outputs against structured, sandbox compilers, math checkers, or tests rather than neural models.
- **Rule Hard-Locks:** Restricts feedback loops to logical, deterministic results, reinforcing correct reasoning steps.

[← Back to README](../README.md)
