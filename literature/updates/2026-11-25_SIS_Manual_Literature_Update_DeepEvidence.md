# SIS Manual Literature Update — 2026-11-25｜DeepEvidence

**Authority:** SIS v0.3.1; SIS Literature Re-Coding Registry v1.3; SIS-LEM-P0 v0.1; ClaimRecord v0.1.  
**Intake:** USER_SUPPLIED_VOR / retrospective manual intake (not a newly published paper today; separate from daily automated batch).  
**Base main:** `cf61e464471c4cf6cac602ca6e6b1afb50b21a2b`.  
**Status:** PRIMARY_VERIFIED / PROVISIONAL_CANDIDATE / FIRST_CODER_ONLY; no permanent SIS-LIT ID, final claim promotion or change to frozen scientific core. Historical chat text was not fully retrievable; this intake follows the repository's documented Registry/P0 conventions and historical 2026-10-24 provenance gate. No SIS-MED repository writes.

## 1. StudyVersionRecord and deduplication

| Field | Value |
|---|---|
| Provisional Study ID | SIS-CAND-20261125-11 |
| Canonical title | Empowering biomedical evidence exploration and synthesis with deep knowledge graph research |
| Authors | Zifeng Wang; Zheng Chen; Ziwei Yang; Xuan Wang; Qiao Jin; Yifan Peng; Zhiyong Lu; Jimeng Sun |
| Venue | Nature Machine Intelligence 8, 1142–1156 (2026) |
| DOI | [10.1038/s42256-026-01266-0](https://doi.org/10.1038/s42256-026-01266-0) |
| PMID / PMC | [42569156](https://pubmed.ncbi.nlm.nih.gov/42569156/) / [PMC13449190](https://pmc.ncbi.nlm.nih.gov/articles/PMC13449190/) |
| Publication status | PEER_REVIEWED / version of record |
| Received / accepted / published | 2026-01-25 / 2026-06-04 / 2026-07-02 |
| Primary source | [Publisher](https://www.nature.com/articles/s42256-026-01266-0); user-provided `s42256-026-01266-0.pdf` (18 pages including Reporting Summary; SHA-256 `8c7d956b7be49851af67f5132714bfbde509c4589c335abc763b5b8d468f2897`) |
| Version lineage | [arXiv:2601.11560](https://arxiv.org/abs/2601.11560), earlier title DeepEvidence: Empowering Biomedical Discovery with Deep Knowledge Graph Research → VOR; same authors/system; one Study, preprint superseded for result extraction; full version history/delta not yet reconciled |
| Full text access | VOR body and main figures read; external Supplementary Information, raw source-data spreadsheets and run traces not independently audited |
| Erratum/retraction status | Not independently established; no such notice surfaced in inspected publisher record |
| Qualification | PRIMARY_VERIFIED for source and first-coder anchored performance claims; independent reproduction and adjudication pending |
| Dedup | Exact DOI, PMID, arXiv ID, title and DeepEvidence variants checked against entire Registry at base; no match. Same-day IDs 01–10 existed; 11 allocated provisionally. No permanent count or audit queue expansion |

**Version conflict:** arXiv text reports 80.0% on LabBench-LitQA2, whereas VOR Fig. 1e reports 64.7% (VOR Methods: 184 questions). Do not pool or silently reconcile. Fig. 1e HLE baseline values differ from Results prose for ToolUniverse and Sonnet; use figure values if compared and flag discrepancy. Fig. 5d gap detection 90.0% and Fig. 5f 89.5% are separately reported, not combined. 

## 2. Paper Understanding（先理解论文，不预设 SIS 结论）

**研究问题。** 生物医学知识分散于文献、数据库和异质知识图谱，单次检索及通用工具调用难以充分覆盖实体、跨库关系、多跳证据及冲突语境。DeepEvidence 研究能否通过有组织的深度研究改善跨来源探索与证据综合。

**方法。** LangGraph 分层 orchestrator–subagent；BFRS 广泛发现候选实体、DFRS 沿引用及实体关联深入探索，由 orchestrator 指定目标、知识库与行动预算；Python sandbox 执行批量 API 查询、数据处理、错误反馈/有界重试；显式 Evidence Graph 保存规范化节点、关系、观察与来源；17 个生物医学知识库/数据库的模块化接入与统一检索接口。BFRS/DFRS 是自主选择路径的研究策略而非固定 BFS/DFS；动态证据图是任务内状态，不是预先融合所有数据库的 GraphRAG，也不是长期自我改进。（Fig. 1；Methods pp.1153–1154）

**实验与结果。** Agent arms 共同使用 GPT-5；比较 Biomni、ToolUniverse、GPT-5 和 Sonnet-4.5 文献检索基线。开放基准（Fig. 1e）：

| Benchmark | N | DeepEvidence | Biomni | GPT-5 |
|---|---:|---:|---:|---:|
| HLE-Medicine | 30 | 40.0% | 20.0% | 3.3% |
| LabBench-LitQA2 | 184 | 64.7% | 48.9% | 50.0% |
| SuperGPQA-Medicine-Hard | 172 | 47.1% | 40.7% | 29.4% |
| TrialPanorama-EvidenceQA | 50 | 96.0% | 84.0% | 72.0% |

Fig. 2–4: 靶点识别 68% vs Biomni 56%；开放靶点优先排序专家评分 1.40 vs 1.15（P<0.001）；机制/通路推理 72% vs 44%；体内代谢通量响应代理任务 80% vs 68%；开放转化验证 1.64 vs 1.46（P<0.05）；临床试验样本量估计 68% vs 20%；联合方案设计 52% vs 36%；替代终点 F1 73.3% vs 60.9%。开放挑战的专家评分不是临床结局。另有证据冲突靶点验证任务（Fig. 2d）。不要按摘要任务数机械合并异质结果。

Fig. 5d: Cochrane 版本间新增研究发现：至少一个真阳性@30 90.0% vs Biomni 50.0%；平均 Recall@30 44.14% vs 30.17%。测试集由结论发生变化的版本对构成，不是无更新/有更新总体监测，也不是完整系统综述。Fig. 5f:

| SystemArm | Precision | Recall | Gap detection |
|---|---:|---:|---:|
| ReAct + MCP | 1.1% | 3.7% | 25.0% |
| ReAct + MCP + CodeExec | 17.8% | 36.8% | 80.0% |
| Orchestrator + ReAct | 15.3% | 33.9% | 70.0% |
| Orchestrator + BFRS-only | 24.5% | 26.5% | 65.0% |
| Orchestrator + DFRS-only | 19.9% | 37.1% | 80.0% |
| DeepEvidence | 38.6% | 44.1% | 89.5% |

Fig. 5g: 人工审查 10 个图谱、316 个节点/关系；provenance validity 100%、normalization 99.7%、claim alignment 93.3%、duplication 0.6%。这些值限于抽查；来源存在/实体规范化不等于主张真实、因果或患者适用性。

**作者的机制解释与创新。** 作者将改善联系到专业化探索策略、工具程序化访问、异质知识互补与持续图谱记忆。与通用 ReAct 对比提示盲目增加 Agent 数量并不可靠。它们是合理机制候选；不是已经被中介干预识别的因果路径。

**局限。** 任务标签部分是 KEGG 拓扑/规则代理而非新湿实验真值；样本量设计、重复运行、同预算与信息访问治理、评审者独立性/一致性仍需核查；外部 API 和 LLM 非确定性影响复现。未隔离 Evidence Graph 的独立效应；作者明确指出冲突证据目前依赖 LLM 解释、缺乏正式概率/不确定性调和；临床前/临床研究任务基准不是临床部署或真实患者获益。补充材料和代码未复跑。

## 3. SIS interpretation（claim routing）

| Primary | Cross-cutting | Framework capability profile | Canonical estimand family | Operational estimand | Provisional CL / I / T | Role |
|---|---|---|---|---|---|---|
| SCF | BGT; CSCI hypothesis only | MI/MEAS/ID/EG/BT | CAUSAL_MECHANISM_EFFECT (package candidate) | BIOMEDICAL_EVIDENCE_EXPLORATION_SYSTEM_PACKAGE_EFFECT | CL1 / I1 / T1 | implementation and negative boundary; benchmark candidate |

- **SCF:** 代码执行与探索策略配置改变任务结果；六臂消融能提供局部配置比较，但同模型不等于相同资源/信息/执行条件。CodeExec 增加操作能力、信息可达性及可能的预算开销；BFRS+DFRS 不是完整 2×2 因子实验。中介尚未识别，CL2 仅候选。
- **SDR:** 实现图谱状态更新、失败反馈与重试；没有受控时间依赖故障传播/恢复估计。仅作为 SDR 实验载体。
- **ASR:** 有任务内规划和预算分配；没有等预算固定策略、随机或 oracle 路由比较，不足以认定 POLICY_VALUE 或 VALUE_OF_INFORMATION 已获验证。
- **CSCI:** 固定 GPT-5 有助于控制模型差异，不构成组件能力×系统机制交互实验。**BGT:** 多任务性能 T1；未建立因果迁移或机制不变性。
- **MOSA / ARSO (auxiliary, not primary Program routing):** 强项 M1/M2/M4/M5/M6/M8/M10；纳排/预算为部分 M3；核查为部分 M7，专家评价不等同运行时 M9。任务证据与元诊断证据分开；A1/A2 支持，A4–A10 的系统级识别、机会、位置、独立修复验证未建立。无需新顶层 primitive。
- **SIS-MED implications:** 研究辅助/benchmark evidence，不是临床疗效或临床自主决策；研究证据→主张→适用性→决策必须分离。MOSA/ARSO 映射只作辅助；未修改 SIS-MED 项目。

## 4. Impact & prioritized experiments

**Impact:** SHARPENS; MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; CorePressure WATCH, ScientificCoreDelta 0; no SPEC_REVISION_CANDIDATE. 推荐 Must Read，尤其 Fig. 5f/5g、Methods 与 Discussion。

1. SCF：固定模型/API 快照/原始证据，匹配 token、工具访问、动作预算，比较代码接口及文本/表格/图谱表示；开放主动检索另估总效应，避免调节后信息误当基线混杂因素。BFRS×DFRS 完整因子实验、随机运行与配对 CI，检验交互和候选中介。
2. SDR：在锁定 evidence graph 注入错误实体、来源失效、冲突、API 故障，测量检测、传播、隔离、恢复轨迹及成本。
3. ASR：在 decision-time evidence 下比较固定/随机/自适应 BFRS、DFRS、反证检索、专家升级、拒答及停止，等预算和独立 Gold 衡量效用。
4. CSCI/BGT：独立测量模型能力，因子交互及跨数据库、任务和机构限制复现；无更新 Cochrane 样本检验误报和覆盖。

## 5. Source and repository record

- [VOR](https://www.nature.com/articles/s42256-026-01266-0), [PubMed](https://pubmed.ncbi.nlm.nih.gov/42569156/), [preprint](https://arxiv.org/abs/2601.11560).
- Author-reported resources: [code](https://github.com/RyanWangZf/BioDSA/tree/main/biodsa/agents/deepevidence), [data](https://huggingface.co/datasets/zifeng-ai/DeepEvidence). No claim of reproducing code/data.
- [Claim-level audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-25_DeepEvidence.md); [candidate ClaimRecords](../evidence-map/claims/2026-11-25_DeepEvidence_candidate_claim_records.jsonl); [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md).
- Main evidence map P0 frozen and permanent audit queue unchanged (candidate is not a permanent ID); audit status remains PENDING_SECOND_CODER / no final CL, Primary or transport promotion.
