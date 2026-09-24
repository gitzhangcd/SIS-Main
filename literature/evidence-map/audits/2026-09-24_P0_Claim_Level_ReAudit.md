# SIS P0 Claim-Level Re-Audit｜2026-09-24

**Authority:** SIS v0.3.1  
**Audit program:** SIS Literature Evidence Map P0  
**Purpose:** advance high-priority causal/mechanistic re-audit backlog using primary-source evidence available in the 2026-09-24 daily run.

## Audit decisions

### SIS-LIT-018｜AgentGrad
- **Primary Program:** ASR
- **Primary estimand:** INTERVENTION_LOCUS_SELECTION_EFFECT
- **Decision:** `CL2 CONFIRMED`
- **Basis:** the method sequentially intervenes on one agent at a time and identifies a target whose modification resolves the failure before extracting the corrective signal. This is stronger than observational attribution.
- **Ceiling:** no CL3 promotion in this audit. The paper supports intervention→outcome change, but does not yet establish a separately measured and manipulated mediator pathway.
- **Transport:** `T1` performance replication across multiple MAS benchmarks; no causal transport test.
- **Evidence role:** controlled causal attribution / regulation fixture.

### SIS-LIT-086｜Flag Game
- **Primary Program:** SDR
- **Primary estimand:** PROPAGATION_EFFECT / collective-dynamics mechanism
- **Decision:** `SPLIT REQUIRED`
  - collective organization/population interventions → `CL2` candidate/defensible effect claims;
  - proposed collapse→polarization→performance pathway → remains `CL3 candidate` pending claim-level mediator audit.
- **Basis:** causal agent patching and population/organization manipulations support intervention effects; statistical-mechanical theory and phase-diagram fit are mechanistic evidence but should not be collapsed into a paper-level CL3 label.
- **Transport:** `T1`; toy-model boundary is explicit, no causal transportability.
- **Evidence role:** mechanism + boundary-condition evidence.

### SIS-LIT-104｜How Strongly Should Task State Influence an LLM Agent?
- **Primary Program:** ASR
- **Primary estimand:** ACTION_SELECTION_EFFECT / influence-policy effect
- **Decision:** `CL2 PROMOTED`
- **Basis:** fixed task rules/model with paired episodes and controlled variation in how strongly task state reaches the agent (display/checklist/directive/enforcement), plus exact dynamic ground truth. This supports causal effects of influence mode within tested settings.
- **Boundary:** state correctness, matcher accuracy, model obedience, task decidability, model scale.
- **Transport:** `T1`; effects reverse across task regimes, which is boundary evidence rather than causal transportability.
- **Evidence role:** controlled regulation effect + negative boundary result.

### SIS-LIT-106｜FIRE
- **Primary Program:** ASR
- **Primary estimand:** SELECTIVE_ACTION_UTILITY / runtime-policy effect
- **Decision:** `CL2 CONFIRMED`
- **Basis:** randomized five-arm experiment separates real failure-informed runtime policies from no-policy, timing-matched sham, and generic verification/reconsideration controls.
- **Mechanism ceiling:** coded corrective behavior supports pathway plausibility, but this audit does not promote to CL3 because mediator manipulation/pathway sufficiency is not established.
- **Transport:** `T1`; multiple model tiers/task sets give replication/performance evidence, not causal transportability.
- **Evidence role:** causal regulation + reliability/capability separation.

## P0 implications

1. Paper-level labels remain too coarse: Flag Game requires claim splitting.
2. Strong controlled intervention is sufficient for CL2 even when the intervention is implemented in natural language.
3. CL3 remains rare because most papers do not independently establish and manipulate mediator pathways.
4. Cross-model/benchmark replication continues to stop at T1/T2; no T3/T4 promotion is warranted.

## Queue actions
- SIS-LIT-018: confirm CL2.
- SIS-LIT-086: split claim; CL2 effect + CL3 mechanism candidate.
- SIS-LIT-104: promote candidate → CL2.
- SIS-LIT-106: confirm CL2.
