# SIS P0 Re-audit｜2026-11-25
Base 900d3b1265cf437f5bf005bc0cb15f8649e1416c; SIS-LEM-P0-v0.1. First coder only; final CL, Primary and transport remain pending independent adjudication. Prior candidate levels are triage, not final. Source qualification improved, no independent reproduction.

## SIS-LIT-070 — Large Language Models Develop Belief State Geometry In-Context
Version: https://arxiv.org/abs/2609.17376v2 (2026-11-13; author reports NeurIPS acceptance, archive not verified); https://arxiv.org/html/2609.17376v2 §§5–6, Appendix I and K. 
- 070-C1: SCF descriptive/performance, MI/MEAS/ID/BT; MEDIATED_MECHANISM_EFFECT candidate; probe R² .83–.99 across six LLMs/40 HMMs, CL1 I1 T1; does not identify use. Boundary: probe split, HMM complexity and layer. Kill: held-out HMM + shuffled labels.
- 070-C2: SCF CAUSAL_MECHANISM_EFFECT, MI/ID/MEAS/BT; patch/steer belief subspace vs control, next-token distribution KL to target; CL1 first-coder ceiling with CL2 candidate I2-local/T1. Appendix K.3.2 contrasts past-consistent, inconsistent and random beliefs; suffix lengths 1,5,10. Kill: magnitude matched unrelated directions and preserve output-level next-token marginals.
- 070-C3: SCF MEDIATED_MECHANISM_EFFECT; MI/ID/BT; Appendix I tests NTP-preserving belief component; early-layer self-repair and probe comparability limitations. I3 pathway candidate, CL1 evidence / CL3 unadjudicated, T1 not invariance. Kill: isolate pathway, test necessity and sufficiency against competing predictor with independent target sequences. No automatic inheritance of CL2→CL3.

## SIS-LIT-055 — When Agents Slow Down
https://arxiv.org/abs/2609.15309v1; 2026-09-14, abstract only; FULLTEXT_PENDING.
- 055-C1: SDR LONG_HORIZON_EFFECT, TD/MEAS/ID/BT; best-so-far Elo vs budget; CL1 I1 T1; four agents, four benchmarks; diminishing returns vs independent sampling. Kill: equal compute, alternative outcome scales, censored trajectory analysis.
- 055-C2: ASR POLICY_VALUE, DR/MEAS/ID/BT; 100M tokens split by inflection point on Polyomino Packing +264 Elo over one long session, +355 over ten short sessions; CL1 I1/T0 local policy comparison, full resource and seed checks pending. Kill: independently estimated inflection on held-out tasks vs equal-budget random restart.
- 055-C3: SCF/ASR hypothesis only, DR/ID/BT; mechanism of sustained improvement vs saturation, CL0 I0 T0; human contest history is not an experimentally matched mechanism comparison. Kill: matched feedback, task, prior knowledge, cost. No causal promotion.

## SIS-LIT-034 — Grounding Agent Memory
https://arxiv.org/abs/2609.11060 (2026-09-10), original abstract; FULLTEXT_PENDING. Fixed task agent, retriever, representation and write authority reported.
- 034-C1: SCF CAUSAL_MECHANISM_EFFECT, MI/EG/MEAS/ID/BT; probing-enabled vs ordinary curator CLBench pass 39→73%, task agent cost $3.38→$1.68; CL1 I2-local candidate/T1. Kill: equal total cost including curator, randomized task worlds.
- 034-C2: ASR VALUE_OF_INFORMATION, DR/EG/ID/MEAS/BT; incremental pre-write evidence vs matched read-only placebo; CL0 unisolated value-of-information claim I0 T0; check real probe outcomes, timing and admissible evidence.
- 034-C3: SCF CSCI hypothesis, CAPABILITY_REGIME_MODERATION candidate; IA/MI/BT/ID; positive comparisons on Sonnet and Opus and six APEX worlds, CL1 I1 T1 multi-context performance not T3. Kill: factorial model capability×probe, world drift, external truth and interaction contrast.

Nine first-coder claim splits; 0 final promotions, 0 T3/T4. All second coder/adjudication pending.
