# SAR-01 Round 5 — LLM-Centric Non-LLM Body, Cognitive Floor, Compensation and Feedback

> **SCIENTIFIC DISCUSSION ONLY / OPEN / NOT FROZEN.** User-selected scope: the primary SIS cognitive core is an LLM/LMM; "strong body" contains non-LLM tools, code execution, structured/scientific knowledge, workflow/state machines, verifiers and safety controls. Stronger LLMs hidden in body are excluded from the core compensation experiment. This note neither changes R5.1 nor approves a new Core scientific identity.

## Candidate research identity

SIS studies *task-, information-, resource- and risk-conditional capability of large-model-centered intelligent systems*, including the causal role of non-LLM external execution capabilities and external knowledge, the cognitive-interface competence needed to exploit them, and the effect of closed-loop system feedback on later model–system coordination.

**Scope caveat:** Traditional machine-learning algorithms may appear as fixed supporting tools or comparators; ordinary internal-model-architecture research is not a primary independent SIS question in this candidate scope. Future multimodal cognitive models should not be excluded solely because they are not text-only LLMs. The requirement of an LLM core is a **proposed scope change**, not a scientific inference from the currently broad R5.1 system ontology.

## Critical distinctions

1. **Cognitive floor is conditional, not parameter size or IQ.** For task/context `Ω`, body `B`, manual `K`, budgets and risk limits, define a feasible region of core models satisfying preregistered success/reliability/viability targets; no universal single threshold is assumed. Candidate probe dimensions: goal/constraint grounding, tool/API binding, multi-step sequencing, output interpretation/verification, exception handling/abstention.
2. **System compensation ≠ internal cognitive equality.** Weak brain + strong body/manual can match a stronger brain + minimal body on a stated task set without the weak model becoming equally good at standalone reasoning. Report system-frontier, safety, costs and task strata, not exact-match output alone.
3. **Externalized execution, knowledge and latent expertise are not the same.** Tools can be deterministic or algorithmic, but body modules with embedded complete task solutions or hidden higher-level planning must be classified and tested separately. Answer-containing manuals, evaluator leakage and stronger model delegation cannot support the core mechanism claim.
4. **Feedback-as-information ≠ memory persistence ≠ parameter learning ≠ recursive self-improvement.** Differentiate within-episode adaptation, persistent system memory, model-weight/policy updates across episodes, and self-modification of improvement machinery.
5. **Ex ante causal role of feedback.** Rewards, validators and training trajectories must be versioned and independent of the locked evaluation set; report potential reward hacking and generalization failure. Different training data/compute/tool exposure must not be silently attributed to internalized capability.

## The three linked hypotheses (unproved)

- **H1 Compensation:** Under specified context and budget, non-LLM execution/knowledge mechanisms improve weak-model system performance and can achieve *pre-registered local non-inferiority* to strong-model/minimal-system reference on some task strata.
- **H2 Conditional floor/interactions:** The compensation effect varies with cognitive-interface skill, task interaction complexity, ambiguity, and external-system capability. Substitution, complementarity, saturation, threshold and null/negative effect are all permitted.
- **H3 Feedback frontier shift:** Training the weak core on source-bound execution feedback changes its tool planning/selection, evidence use, verification and recovery competence, and shifts the feasible system-capability region on held-out tools/tasks, over and above equivalent-budget generic training.

## Suggested factorial structure

- Cognitive core: weaker and stronger frozen open-weight model versions (capability measured independently, not by model ID).
- Body: minimal tools vs strong *non-LLM* execution/workflow/verification, with no hidden stronger LM.
- Manual: minimal vs versioned knowledge/evidence and executable guides.
- Feedback learning: frozen weak model vs feedback-trained weak model vs equal-budget generic-training control. Evaluate both with/without the body for internalization attribution.
- Compare matched-budget, budget-capped, actual resource usage and safety/viability; do not equate the concepts. Use fixed evaluator, blinded held-out tasks, task-family grouping, repeated stochastic runs and confidence intervals.
- Use prospective task difficulty stratification by dependency depth, intrinsic/semantic ambiguity, recovery needs, novelty, risk and information gaps.
- For the strongest hypothesis, test *non-inferiority with pre-registered margin* and separate cost/risk bounds, not merely "no significant difference".

## Adversarial kill tests

1. **Hidden strong-model delegation:** a body contains a stronger reasoning model ⇒ compensation claim fails for designated non-LLM-body arm.
2. **Precompiled solution:** strong body simply holds a hard-coded solution for evaluation tasks ⇒ cannot claim general-purpose compensation.
3. **Manual gold leakage:** guide contains held-out answer/evaluator criteria ⇒ invalid independent performance claim.
4. **Weak core can't route:** body improves but catastrophic task grounding/selection/recovery errors remain ⇒ cognitive floor persists.
5. **Excess computation:** extra model calls, retries, time and human effort explain gains ⇒ causal mechanism not independently identified.
6. **No cross-task transfer:** feedback training helps seen tool/task only ⇒ do not claim generalized internalized tool-use capability.
7. **Reward/evaluator hacking:** altered grader or reward proxy drives apparent gain ⇒ not valid capability growth.
8. **Safety and reliability collapse:** average accuracy up but high-severity failures or worst strata worsen ⇒ no general systems-level improvement claim.

## Literature touchstones

- Toolformer (NeurIPS 2023): https://papers.neurips.cc/paper_files/paper/2023/hash/d842425e4bf79ba039352da0f658a906-Abstract-Conference.html
- ReAct (ICLR 2023): https://arxiv.org/abs/2210.03629
- Rethinking Scale: Deployment Trade-offs of Small Language Models under Agent Paradigms (ACL Industry 2026): https://aclanthology.org/2026.acl-industry.123/
- Beyond Accuracy: A Cognitive Load Framework for Mapping the Capability Boundaries of Tool-use Agents (AAAI 2026): https://ojs.aaai.org/index.php/AAAI/article/view/40650
- ToolSandbox (Apple Research): https://machinelearning.apple.com/research/toolsandbox-stateful-conversational-llm-benchmark
- ToolRL (NeurIPS 2025): https://proceedings.neurips.cc/paper_files/paper/2025/hash/97c5b2707228e7e3fb67e4ecc2e0e607-Abstract-Conference.html
- Tool-Induced Myopia (ACL 2026): https://aclanthology.org/2026.acl-long.1951/

## Open science-owner issue (no adoption)

For the primary body-manual compensation program, should **pre-composed workflows with high-level decision logic** count as strong non-LLM body, provided their authorship, coverage, task-specificity and procedural knowledge are explicitly measured? Candidate resolution: YES, but stratify body intelligence into atomic execution tools, generic workflow/verification scaffolds and domain precompiled procedures. Require novel task combinations / perturbations and report exactly where the cognitive work was performed.

**Status:** SAR-01 OPEN; no master edit, no schema change, no empirically validated cognitive threshold or compensation law.
