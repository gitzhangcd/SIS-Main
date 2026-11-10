# SIS Daily Literature Update｜2026-11-10

Authority: SIS v0.3.1 Master, Registry v1.3, P0 Audit Queue, 2026-11-09 update and audit. Search as of Tuesday Nov 10 Asia/Shanghai. arXiv cs.AI public listing Monday Nov 9: 397 entries, 94 new submissions; selected ten original preprints submitted Nov 5–6, discovered Nov 10, not first posted on Nov 10.

Search: arXiv, ACL Anthology, OpenReview/NeurIPS and relevant official research/technical sources. No independent new peer-reviewed version preferred over these ten; author workshop note not peer-reviewed verification. Community analysis DISCOVERY_ONLY only. Exact arXiv ID/title dedup against 145 permanent + synced temporary Registry. Oct 9–23 unsynced historical global lineage pending; no permanent IDs added.

## 10 original high-value preprints

### 1. Knowing When to Intervene: Causal Evaluation of AI Agents
- Original source: https://arxiv.org/abs/2611.09792; submitted 2026-11-06; priority undefined
- Novelty / quantitative primary evidence: 检查实际随机分配、序列可交换性和支持集覆盖；干预成本、干预资格与状态记录可能影响因果估计，不能直接推广到真实部署。
- SIS route: Primary ASR; Cross BGT; Framework DR/TD/ID/MEAS/BT; Estimand DYNAMIC_RANDOMIZED_INTERVENTION_POLICY_VALUE
- Maturity CL0 methods + CL1 empirical, local CL2 candidate; Identification I2-local provisional; Transport T1; evidence role Measurement / conditional policy effect
- Limits and confounders: SHARPENS ASR; intervention timing/state condition.
- SIS scientific impact: Must Read

### 2. s³: Simple Scaling of Swarms via Cooperative Multi-agent RL
- Original source: https://arxiv.org/abs/2611.08615; submitted 2026-11-05; priority undefined
- Novelty / quantitative primary evidence: 结果对任务基数、信息私有性、模型能力、训练预算敏感；跨规模性能不证明T3因果迁移。
- SIS route: Primary SCF; Cross CSCI/BGT; Framework MI/IA/DR/MEAS/ID/BT; Estimand LEARNED_INFORMATION_SHARING_POLICY_BY_TEAM_SCALE
- Maturity CL1; local CL2 candidate; Identification I1/I2-local; Transport T2-performance-only; evidence role Component organization / performance transfer
- Limits and confounders: SHARPENS SCF/CSCI; adaptive disclosure.
- SIS scientific impact: Must Read

### 3. NormGym: Evaluating Normative Competence through Social Interaction
- Original source: https://arxiv.org/abs/2611.08613; submitted 2026-11-05; priority undefined
- Novelty / quantitative primary evidence: 合成规范环境与实际制度不同；观察惩罚和自身被惩罚所提供证据不同；不能从一次合规证明可迁移规范学习。
- SIS route: Primary SCF; Cross CSCI/BGT; Framework MI/TD/IA/MEAS/ID/BT; Estimand HIDDEN_SOCIAL_NORM_INDUCTION_AND_COMPLIANCE_TRANSFER
- Maturity CL1; Identification I1; Transport T1; evidence role Negative capability formation / norm boundary
- Limits and confounders: SHARPENS SCF; norm discovery versus compliance.
- SIS scientific impact: Must Read

### 4. Pdb or Not to Be: Comparing Debugging Interfaces With Pass_X@k
- Original source: https://arxiv.org/abs/2611.08666; submitted 2026-11-05; priority undefined
- Novelty / quantitative primary evidence: 只有两个模型与有限复跑，随机性仍未充分消失；作者Workshop接收声明未由正式论文集核验，按预印本记录。
- SIS route: Primary ROUTING_ABSTAIN; Cross BGT; Framework MI/MEAS/ID/BT; Estimand STOCHASTIC_DEBUG_INTERFACE_COMPLEMENTARITY_PASSXK
- Maturity CL1; local CL2 candidate; Identification I2-local; Transport T1; evidence role Negative apparent tool complementarity / measurement
- Limits and confounders: CHALLENGES tool diversity equals independent capability assumption.
- SIS scientific impact: Must Read

### 5. Cancellation Is Not Enough: What Retries Leave Behind in an Overloaded LLM Engine
- Original source: https://arxiv.org/abs/2611.08684; submitted 2026-11-05; priority undefined
- Novelty / quantitative primary evidence: 单推理引擎及若干调度设置；取消的API响应不等于资源实际释放；需测量最终交付、成本计数缺失及服务公平性。
- SIS route: Primary SDR; Cross CSCI/BGT; Framework TD/DR/EG/MEAS/ID/BT; Estimand RETRY_CANCELLATION_COALESCING_POST_OVERLOAD_RECOVERY
- Maturity CL1; local CL2 candidate; Identification I2-local; Transport T1; evidence role Negative system recovery / hidden resource cost
- Limits and confounders: SHARPENS SDR; hidden executor recovery state.
- SIS scientific impact: Must Read

### 6. Aligning, Fast and Slow: A Control-Theoretic Oversight Framework for Long-Horizon Trajectories and Maintained Deployments
- Original source: https://arxiv.org/abs/2611.08781; submitted 2026-11-05; priority undefined
- Novelty / quantitative primary evidence: 理论保证依赖状态充分和控制权限；编码任务解题数33/120低于对照35/120，必须报告防护带来的能力成本。
- SIS route: Primary ASR; Cross CSCI/BGT; Framework DR/TD/EG/ID/MEAS/BT; Estimand FAST_ACTION_SLOW_PERSISTENT_UPDATE_OVERSIGHT_BUDGET_VALUE
- Maturity CL0 conditional theory + CL1 empirical; Identification I0/I2-local; Transport T1; evidence role Two-timescale regulation / viability boundary
- Limits and confounders: SHARPENS ASR; action and update governance.
- SIS scientific impact: Must Read

### 7. When F1 Is Not Enough: Auditing Codebooks for LLM-Assisted Annotation
- Original source: https://arxiv.org/abs/2611.08846; submitted 2026-11-06; priority undefined
- Novelty / quantitative primary evidence: 修订会改变被测构念，不能直接把前后F1差异归咎于模型；独立Gold和双盲标签必须审查，当前仅两套规范。
- SIS route: Primary ROUTING_ABSTAIN; Cross BGT; Framework MEAS/EG/ID/BT; Estimand CODEBOOK_RULE_REVISION_VS_ANNOTATOR_ERROR_HELDOUT_VALIDITY
- Maturity CL1; local CL2 candidate; Identification I1/I2-local; Transport T1; evidence role Measurement instrument defect / annotation validity
- Limits and confounders: SHARPENS MEAS/EG; codebook truth ownership.
- SIS scientific impact: Must Read

### 8. Scout Before You Route: Predicting Task Success and Token Count from a Small LLM Prefill
- Original source: https://arxiv.org/abs/2611.09028; submitted 2026-11-06; priority undefined
- Novelty / quantitative primary evidence: 长度预测误差、缓存、定价、探针开销与成功率校准均影响真实性价比；非推理模型上的收益较弱。
- SIS route: Primary ASR; Cross CSCI/BGT; Framework DR/MEAS/ID/BT; Estimand QUERY_CONDITIONAL_MODEL_COST_SUCCESS_ROUTING_NET_VALUE
- Maturity CL1; local CL2 candidate; Identification I1/I2-local; Transport T2-performance-only; evidence role Resource-aware routing / conditional policy
- Limits and confounders: SHARPENS ASR; query-conditional costs.
- SIS scientific impact: Must Read

### 9. BMMS: Policy-Conditioned Measurement of Behavioral Compliance in Language Models
- Original source: https://arxiv.org/abs/2611.09147; submitted 2026-11-06; priority undefined
- Novelty / quantitative primary evidence: 规则抽取和解释均可能偏差；分数稳定不代表被测行为满足真实权限；自然语言合规不能替代工具动作审计。
- SIS route: Primary ROUTING_ABSTAIN; Cross BGT; Framework MEAS/EG/ID/BT; Estimand POLICY_OBLIGATION_JUDGE_INSTRUMENT_TARGET_SCORE_INVARIANCE
- Maturity CL0 measurement contract + CL1; Identification I1; Transport T1; evidence role Measurement instrument / obligation coverage
- Limits and confounders: SHARPENS MEAS; evaluator scores versus true obligations.
- SIS scientific impact: Must Read

### 10. Can Agentic Systems Close the Gap in Radiology with Production AI Tools?
- Original source: https://arxiv.org/abs/2611.09836; submitted 2026-11-06; priority undefined
- Novelty / quantitative primary evidence: 临床报告模拟工具正确输出，不含真实设备误诊、患者结局和部署风险；用目标报告生成的Oracle计划并非真实可用上界。
- SIS route: Primary SCF; Cross CSCI/BGT; Framework MI/IA/EG/MEAS/ID/BT; Estimand MODALITY_TOOL_COVERAGE_BY_ORCHESTRATOR_CLINICAL_FINDING_RECALL
- Maturity CL1; local simulated CL2 candidate; Identification I2-local simulated; Transport T1; evidence role Negative clinical tool availability / model orchestration boundary
- Limits and confounders: SHARPENS SCF/CSCI; availability versus actual ability.
- SIS scientific impact: Must Read

## P0 first-coder audit
- Detailed record: ../evidence-map/audits/SIS_P0_Reaudit_2026-11-10.md ; 086, 087, 097, nine distinct claims. Abstract-level verified only; second coder and full text pending, zero promotions.

## Five key implications and experiment candidates
1. Randomized dynamic intervention under sequential eligibility: estimate state-conditioned policy value, compare nonintervention and full intervention with matched budget and positivity checks.
2. Information sharing/social norm capability: factor team size by private/shared information and hidden norm observation versus intervention, including pre-registered heldout compositions.
3. Tool complementarity can be seed noise: compare bash/debugger with many reruns, pass_X@k, matched scaffolds and compute; do not infer independent capability from a single run.
4. Fast actions and slow persistent updates require distinct authority rules; runtime cancellation, retries and coalescing must track true resource use, delivery, correct requests rejected and regression.
5. Codebook and compliance measurement must be separately audited: CodebookVersion by IndependentGold by Judge, and radiology ToolAvailability by ExecutorSelection with true-device false-negative realism. Probe-cost conditional routing is secondary.

## Formal SIS Impact Decision
MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA. Real pressure on identification of time-varying policy value, sampling variance, codebook validity and resource recovery, all expressible by SCF/SDR/ASR with CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG. ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO; no confirmed T3/T4.
