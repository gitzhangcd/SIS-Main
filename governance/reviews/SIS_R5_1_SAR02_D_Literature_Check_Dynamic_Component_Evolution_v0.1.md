# SAR-02-D Literature Check v0.1 — Feedback-Driven System Component and Structure Evolution

> **2026-10-28 — Evidence review only / SAR-02-D owner decision still PENDING / SAR-02 OPEN / R5.1 Master UNCHANGED.**  
> User scientific position: “条件性双视图是必要的，因为现在有不少智能系统的研究已经可以根据反馈自主决定增加或者减少组件了。” User requested verification against `https://github.com/gitzhangcd/SIS-Main/tree/main/literature`. This record supports an evidence-informed discussion of option A, **not** a completed formal science-owner decision receipt, a normatively adopted `C_t`, or an empirical SIS law.

## 1. Source audit boundaries

**GitHub main/literature actually read:**
- [Permanent registry, 145 records](https://github.com/gitzhangcd/SIS-Main/blob/main/literature/SIS_v0.3.1_Literature_Re-Coding_Registry.md), blob `3d83a56a7454d41ac6b0f3b271b22c8fb3d85a79`.
- [2026-10-25 discovery and primary-source notes](https://github.com/gitzhangcd/SIS-Main/blob/main/literature/updates/2026-10-25_SIS_Daily_Literature_Update.md), blob `a0452351660c20136e07a41b84eff3e4c8f0c577`.
- [2026-10-26 discovery notes](https://github.com/gitzhangcd/SIS-Main/blob/main/literature/updates/2026-10-26_SIS_Daily_Literature_Update.md), blob `8189f65f7b63bac30a679312da74370a5b35ec70`.
- [P0 evidence map](https://github.com/gitzhangcd/SIS-Main/blob/main/literature/evidence-map/SIS_Literature_Evidence_Map_P0.md) and [P0 audit queue](https://github.com/gitzhangcd/SIS-Main/blob/main/literature/evidence-map/SIS_P0_Audit_Queue.csv) reviewed for source and claim-maturity governance.

**Source-status warning:** Permanent registry contains paper-level first-pass coding, not final claim-level Gold. `SIS-CAND-20261025-05` is a **provisional, not permanent SIS-LIT ID**; registry labels its source claim `CL1; local CL2 candidate; T0`. Do **not** report 145 confirmed causal findings, or 7 proven dynamic-component-birth papers.

## 2. Primary references: what specifically changes?

| Repo ID | Study / primary source | What primary source supports | Change class | Does it prove creation/deletion of independently identified components? |
|---|---|---|---|---|
| `SIS-CAND-20261025-05` | [Conservative Meta-Agent Search: Architecture Adaptation under Non-Stationarity](https://arxiv.org/abs/2610.31436), 2026-10-22 preprint | Typed graph edits to proposed agent architectures, feedback from paired shadow replay and conservative promotion/rollback; contracts to near-single-agent teams when additional workers lack value; 96 designed simulated streams | **Architecture search / active worker population contraction; potentially membership-changing proposal** | **No general guarantee** of novel independent model/agent identity creation or real deployment. Strongest direct current repo example for adaptive architecture cardinality; designed simulator and input worker capabilities |
| `SIS-LIT-111` | [Learning to Orchestrate Agents in Natural Language with the Conductor](https://arxiv.org/abs/2512.04388), ICLR 2026; [authors](https://sakana.ai/learning-to-orchestrate/) | RL-learned controller chooses worker agents from existing pool, conditions instructions and communication topology; simpler tasks use one, harder tasks spawn multi-stage planner/coder/verifier workflows | **Runtime team selection and active instances/topology** | **No** newly trained/unbounded model identity; composes existing workers. Dynamic population in *active* sense supports M1 |
| `SIS-LIT-052` | [FAMA](https://aclanthology.org/2026.findings-acl.1716/), ACL Findings 2026 | Failure-trajectory-based orchestration activates a minimum subset of specialized agents before action | **Selective activation/deactivation of existing specialists** | **No** birth/death of novel components shown in abstract; M1 strongly sufficient for known pool |
| `SIS-LIT-028` | [MASkills](https://aclanthology.org/2026.findings-emnlp.1453/), EMNLP Findings 2026; [author mechanism](https://darl-genai.github.io/LangMARL_homepage/maskills.html) | Failure and skill credit drive refinement, **induction (new skill)**, consolidation (merge), and **pruning (delete low-utility skill)**, accepted via held-out validation/rollback | **Persistent skill-library membership adds/removes** | **Yes for skill artifacts as independently tracked capability resources**, but **not automatically** for independently executing agent instances; role/identity convention determines whether skills count as SIS Components vs knowledge/procedural state |
| `SIS-LIT-019` | [Procedural Graphs](https://arxiv.org/abs/2609.09153), Sep 2026 preprint | Failure/success traces refine executable procedural graph topology and attributes with held-out gate | **Procedural network topology mutation** | **Not evidence** that separate agent members were born or deleted; dynamic graph relation/state fits R_t and/or procedural artifacts |
| `SIS-LIT-021` | [SE-GoS](https://arxiv.org/abs/2609.08228), Sep 2026 preprint | Execution-trace-driven discovery/pruning of **skill relationships**, edge weights and descriptions; underlying skill library and retrieval pipeline fixed | **Graph edges changed; skill membership held fixed** | **No**. In fact this is a negative discriminator against conflating relation-pruning and component-removal |
| `SIS-LIT-102` | [Grow the Harness, Not the Context](https://arxiv.org/abs/2609.26760), Sep 2026 preprint | Failure-guided durable changes accumulate in reusable executable harness code, with held-out gates and rollback | **Persistent procedural code/control structure growth** | **Conditional:** new software functionality can be a new component if separately identity-bearing/invocable/authorized; source abstract alone does not establish newly independent process/agent identities |
| `SIS-CAND-20261026-08` | [Learning Who Talks to Whom](https://arxiv.org/abs/2610.25851), Oct 2026 preprint | Role-conditioned selection and communication topology adapts, tested on nine benchmarks (local first-coder). | **Relation/communication topology selection** | **No** unique evidence for component membership changes; mostly `R_t` and `π_t` |

## 3. Five distinctions SAR-02 must preserve

1. `RELATION_EDIT`: graph edges `R_t` change; `C` may stay constant — e.g. SE-GoS and communication topology scheduling.
2. `ACTIVATE/DEACTIVATE`: chosen subset of an existing known worker/skill pool changes — M1 `C^*` + `active_t` is generally adequate when identity/provenance stable.
3. `SKILL_INDUCE/PRUNE`: bounded skill **artifacts** are minted/merged/pruned; whether such a skill is `Component`, `Knowledge`, or `ProceduralState` must be defined by the system boundary and intervention target. MASkills clearly establishes capability-resource membership evolution.
4. `PROGRAM_GENERATE/REWRITE`: executable control/handler code evolves; persistent component identity is not inferable from code changes alone.
5. `NEW_COMPONENT_IDENTITY_CREATE/RETIRE`: autonomous creation/retirement of *distinctly addressable, authority-bearing capability components*. The checked GitHub records **do not yet provide robust, independently validated general evidence** for this unrestricted claim. CMAS provides architecture/topology adaptation in a simulator, but no population-wide independent identity guarantee.

Therefore the user thesis is **SUPPORTED AS A CLASS OF DYNAMIC SYSTEM ARCHITECTURE AND CAPABILITY-RESOURCE EVOLUTION**, but **NOT ESTABLISHED IN ITS STRONGEST OPEN-WORLD INDEPENDENT-IDENTITY INTERPRETATION**.

## 4. Scientific implications for the SAR-02-D option A decision

Evidence favors **conditional dual-view** as the appropriate *audit research posture*:

- **M1** when `C^*` is a justified known set of potential workers/tools/skill IDs and changing active members/edges is the estimand. `active_t`, version, effective relations, author provenance and true runtime costs must be measured.
- **M2** should remain an **open-world membership representation candidate** if persistent creation/deletion of distinct authority-bearing component identities becomes relevant; avoid declaring `C_t` normatively adopted based on existing papers.
- Two scientific axes should be measured separately: **`effective active population/topology`** and **`identity-bearing component birth/death`**. Neither agent count nor graph edges alone determines system intelligence.
- Across representation regimes, require `ComponentIdentityMap`, `LifecycleEventLog`, `AuthorizationMap`, `InterventionCorrespondence` and `EstimandPreservation` where relevant. These are **review criteria**, not added schema fields or ontology primitives.
- Under feedback, architecture/resource change can be **ASR** if primary estimand is information-conditioned action-policy value; **SCF** if effect of adding/removing component is experimentally manipulated; **SDR** if effect of a time-ordered topology/identity transition is the primary estimand. **No forced program** without primary claim/estimand.

**Key pressure tests for SAR-02/SAR-04:** `activate_existing_agent` vs `spawn_new_identity`; `remove_graph_edge` vs `delete_skill`; `rewrite_code` vs `mint_new_invocable_tool`; `delete_then_recreate` vs `disable_then_enable`; hidden more powerful model delegation; equal inference-budget/control and independent evaluation. Log `birth/disable/retire/replace/rewire` as different events.

## 5. Evidence qualification and decision status

- User's preference strongly supports **Option A** in SAR-02-D, but **this audit note does not itself record a formal A decision**; the formal docket `SAR-02-D-DEC-001` remains owner-choice PENDING until the user elects to formalize it after source review.
- `G-01...` and `G-02` semantic clarifications remain proposals; G-O/G-E not executed.
- R5.1 official Master and `main` are unchanged; draft review PR #4 remains open.
- No universal empirical law that feedback necessarily improves system intelligence, increases agent count, or creates new component identity is asserted.
