# Eight-Week AI Engineer Study Checklist

AI 工程师 8 周学习打卡清单

Prepared on November 19, 2026, for a developer with 10 years of software engineering experience preparing for U.S. Senior AI / Agent Engineer roles.

整理于 2026 年 11 月 19 日，适用于具有 10 年软件开发经验、准备申请美国 Senior AI／Agent Engineer 岗位的工程师。

The final objective is a complete AI product for developers or individual users, validated by paying customers and positive operating profit over a documented period. Plan for 8–10 hours per week, developing agent mechanisms, systematic evaluation, and production reliability through that product. Time allocations, exercises, and acceptance criteria are learning recommendations. The course labs have yet to be run as part of preparing this checklist.

最终目标是面向开发者或个人用户，完成一个有真实付费客户、在明确统计周期内经营利润为正的完整 AI 产品。每周安排 8–10 小时，通过这个产品依次掌握 Agent 机制、系统化评测和生产可靠性。时间分配、练习和验收标准属于学习建议。本清单整理过程中尚未实际运行课程实验。

For job requirements and background research, see the [companion guide](AI工程师岗位要求与8周学习计划.md).

岗位要求与背景调研见[配套指南](AI工程师岗位要求与8周学习计划.md)。

## How to Check In

如何打卡

- Check a study item after completing its reading or exercise. Check the weekly acceptance items after recording evidence such as a commit, trace, report, or demo.

  完成阅读或练习后勾选学习项。记录提交、执行轨迹、报告或演示等证据后，再勾选每周验收项。
- Use the evidence fields at the end of each week. Repeat an exercise when its acceptance condition fails, then record the result of the retry.

  使用每周末的证据记录栏。验收失败时重新练习，并记录重试结果。
- Required items form the recommended core. Optional items deepen a topic. Choose one cloud deployment route in Week 7.

  必学项组成推荐主线，选学项用于深入。第 7 周选择一条云部署路线。

## Course and Resource Checklist

课程与资料清单

There are 15 resource entries when the three LangGraph reference pages are counted together. The core has 10 required entries plus one of the two cloud routes. Three entries are optional. Week 8 consolidates earlier work.

将三篇 LangGraph 参考文档合并计数后，共有 15 项资料。主线包括 10 项必学和两条云路线中的一条，另有 3 项选学。第 8 周整合前面成果。

- [ ] **R01 · Required · Week 1** — Anthropic, Building effective agents. Study workflow and agent patterns and their trade-offs. [Article](https://www.anthropic.com/research/building-effective-agents)

  **必学 · 第 1 周** — Anthropic，构建高效 Agent。学习工作流、Agent 架构及其取舍。
- [ ] **R02 · Required · Week 1** — Anthropic, Tool use with Claude. Follow the current tool definition, invocation, result handling, and tutorial sections. [Documentation](https://platform.claude.com/docs/en/agents-and-tools/tool-use/overview)

  **必学 · 第 1 周** — Anthropic 工具调用文档。学习工具定义、调用、结果处理和当前教程。
- [ ] **R03 · Required · Week 1** — Anthropic, Writing effective tools for agents. Focus on schemas, descriptions, useful responses, and token efficiency. [Article](https://www.anthropic.com/research/writing-tools-for-agents)

  **必学 · 第 1 周** — Anthropic 工具设计文章。重点学习 schema、描述、有效返回内容和 token 效率。
- [ ] **R04 · Required · Week 1** — Anthropic, Effective context engineering for AI agents. Study context selection, history, retrieval, and long-running tasks. [Article](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents)

  **必学 · 第 1 周** — Anthropic 上下文工程文章。学习信息选择、历史、检索与长任务上下文。
- [ ] **R05 · Optional · Weeks 1–2** — DeepLearning.AI, Agentic AI, taught by Andrew Ng. Approximately 7 hours 45 minutes of video. [Course](https://www.deeplearning.ai/courses/agentic-ai)

  **选学 · 第 1–2 周** — 吴恩达 Agentic AI 课程，约 7 小时 45 分钟视频。适合希望系统观看设计模式讲解时补充学习。
- [ ] **R06 · Required · Week 2** — LangChain Academy, Introduction to LangGraph — Python. Approximately 6 hours of video. Prioritize state, memory, streaming, and human-in-the-loop exercises. [Course](https://academy.langchain.com/courses/intro-to-langgraph)

  **必学 · 第 2 周** — LangChain 官方 LangGraph 课程，约 6 小时视频。优先完成状态、记忆、流式响应和人工介入练习。
- [ ] **R07 · Required · Week 3** — DeepLearning.AI × Arize AI, Evaluating AI Agents. Approximately 2 hours 16 minutes. [Course](https://www.deeplearning.ai/courses/evaluating-ai-agents)

  **必学 · 第 3 周** — DeepLearning.AI 与 Arize 联合评测课程，约 2 小时 16 分钟，学习追踪、评分器和实验。
- [ ] **R08 · Required · Week 3** — Anthropic, Demystifying evals for AI agents. Study tasks, outcomes, graders, repeated trials, and regression evaluation. [Article](https://www.anthropic.com/research/demystifying-evals-for-ai-agents)

  **必学 · 第 3 周** — Anthropic Agent 评测指南，学习任务、结果、评分器、重复运行和回归评测。
- [ ] **R09 · Required · Weeks 3–4** — OpenAI, Evaluation best practices. Apply objective definition, representative datasets, human calibration, and continuous evaluation. [Guide](https://developers.openai.com/api/docs/guides/evaluation-best-practices)

  **必学 · 第 3–4 周** — OpenAI 评测最佳实践，学习目标定义、代表性数据、人工校准和持续评测。
- [ ] **R10 · Optional · Week 4** — Microsoft Learn, Evaluate and optimize AI agents through structured experiments. Approximately 1 hour 6 minutes. [Module](https://learn.microsoft.com/en-us/training/modules/evaluate-optimize-agents/)

  **选学 · 第 4 周** — 微软结构化实验课程，约 1 小时 6 分钟，补充实验版本组织和评分规则设计。
- [ ] **R11 · Required · Week 5** — LangGraph reference set. Read persistence, fault tolerance, and interrupts together. [Persistence](https://docs.langchain.com/oss/python/langgraph/persistence) · [Fault tolerance](https://docs.langchain.com/oss/python/langgraph/fault-tolerance) · [Interrupts](https://docs.langchain.com/oss/python/langgraph/interrupts)

  **必学 · 第 5 周** — LangGraph 持久化、故障容错和人工中断文档，重点理解恢复时的执行与副作用。
- [ ] **R12 · Required selected modules · Weeks 5–6** — Microsoft Learn, Monitor, evaluate, and operate multi-agent AI solutions in Azure. Prioritize observability, performance and cost, and incident response. [Learning path](https://learn.microsoft.com/en-us/training/paths/aaai-4-monitor-evaluate-operate-multi-agent-ai-solutions-azure/)

  **必学重点模块 · 第 5–6 周** — 微软高级学习路径。重点学习可观测性、性能与成本，以及生产事故处理，并将概念应用到自己的项目。
- [ ] **R13A · Cloud route A · Week 7** — AWS, Getting started with AgentCore. Work through runtime, identity, memory, tools, and observability. [Workshop](https://catalog.workshops.aws/agentcore-getting-started/en-US)

  **云路线 A · 第 7 周** — AWS AgentCore 官方实践，学习运行时、身份、记忆、工具与可观测性。与 R13B 二选一。
- [ ] **R13B · Cloud route B · Week 7** — Google Skills, Build and Deploy Agents in Production. Approximately 45 minutes of introductory material. [Course](https://www.skills.google/paths/3802/course_templates/1633)

  **云路线 B · 第 7 周** — Google Agent 生产部署课程，约 45 分钟入门内容，搭配自己的云部署练习。与 R13A 二选一。
- [ ] **R14 · Optional · Week 7** — Google Cloud, Agent Starter Pack. Inspect and adapt its deployment, CI/CD, evaluation, and observability templates. [Repository](https://github.com/GoogleCloudPlatform/agent-starter-pack)

  **选学 · 第 7 周** — Google 官方工程模板。选择 Google 路线时推荐参考其部署、CI/CD、评测和可观测性实现。

## The Project Used Throughout

贯穿八周的项目

Build one narrowly scoped product for developers or individual users. In Week 1, compare recurring tasks that you can investigate directly, such as explaining failed agent traces, turning technical reading into contextual practice, or reviewing AI engineering interview answers. These are discovery hypotheses. Select the product from observed workflows, accessible samples, and willingness to try and pay.

面向开发者或个人用户构建一个范围明确的小产品。第一周比较自己能够直接调研的重复任务，例如 Agent 失败轨迹分析、技术阅读后的情境练习、AI 工程面试回答复盘。这些是待验证的需求假设，具体产品根据真实工作流程、可获得的样本，以及试用和付费意愿确定。

The order-support example in the engineering exercises provides a concrete implementation reference. Apply the same tool, state, approval, evaluation, and recovery exercises to the selected product, and record the corresponding user task. Define a complete input-to-deliverable workflow with onboarding, usage limits, payment or paid-pilot terms, support, and a repeat-use path.

工程练习中的订单售后示例提供具体实现参考。将相同的工具、状态、确认、评测和恢复练习映射到所选产品，并记录对应用户任务。完整产品需要覆盖输入到交付结果的流程，以及引导、用量限制、支付或付费试点约定、支持和重复使用路径。

## Commercial Outcome and Evidence

商业目标与证据

Use eight weeks as the first build-and-validation cycle. A completed learning cycle and a commercially validated product have separate evidence. If profitability remains unverified, record the gap and extend or adjust the product experiment.

八周作为第一轮开发与验证周期。完成学习周期和完成商业验证分别记录证据。若盈利尚未验证，记录缺口并延长或调整产品实验。

- [ ] Identify a specific user, recurring task, current alternative, and measurable benefit using real conversations and task samples.

  通过真实交流与任务样本，明确用户、重复任务、现有替代方案和可衡量收益。
- [ ] Deliver a complete core workflow that a target user can complete, with result review, failure handling, onboarding, support, and clear paid terms.

  交付目标用户能够完成的核心流程，具备结果检查、失败处理、引导、支持和清晰付费约定。
- [ ] Record payment from a target customer and actual delivery. Keep the agreed scope, transaction evidence, refunds, and customer feedback.

  记录目标客户的真实付款与实际交付，保留约定范围、交易凭证、退款和反馈。
- [ ] Measure repeat use and renewal or repeat-purchase decisions over an observation period appropriate to the task frequency.

  按任务发生频率确定观察周期，记录重复使用、续费或再次购买的决定。
- [ ] Demonstrate positive operating profit for a stated period, including product revenue, refunds, payment fees, model and tool calls, hosting, storage, acquisition spending, and delivery/support labor.

  在明确周期内验证经营利润为正，核算产品收入、退款、支付手续费、模型和工具调用、托管、存储、获客支出，以及交付和支持人工。
- [ ] State how founder labor is valued. Report one-time development hours and spending separately and estimate the time needed to recover them at the observed profit rate.

  明确自己的人工时间如何计价，单列一次性开发时间与支出，并按实测利润估算收回投入所需时间。

Operating profit for the observation period equals product revenue earned from delivered service, less refunds and all operating costs above. Distinguish prepaid cash from revenue earned during the period. Use actual invoices and time records where available, identify estimates, and report both per-successful-task cost and period profit.

观察周期经营利润等于已交付服务对应的产品收入，减去退款和上述全部经营成本。区分预收现金与当期已交付服务收入。有账单和工时记录时使用实测数据，标明估算部分，同时报告单次成功任务成本和周期利润。

Start with approximately two hours of focused study, five hours of development and evaluation, and two hours of user contact, sales, and review each week. Reallocate time to the current product blocker. Optional courses can replace study time within that budget.

每周先按约两小时针对性学习、五小时开发评测、两小时用户接触销售与复盘安排，并根据产品当前阻碍调整。选学课程占用这份预算内的学习时间。


## Week 1 — Agent Mechanisms and Tool Use

第 1 周 — Agent 机制与工具调用

Use 75 minutes on each weekday and two hours on each weekend day, approximately 10 hours in total. Study R01–R04. R05 is optional extra viewing.

工作日每天 75 分钟，周末每天 2 小时，共约 10 小时。学习 R01–R04，R05 可按需要补充观看。

### Daily Practice

每日练习

- [ ] **Day 1** — Read R01. Draw the execution flow and identify decisions made by the model, application, and user. Explain two architectural choices.

  **第 1 天** — 阅读 R01，画执行流程，标明模型、应用和用户各自负责的决策，并解释两个架构选择。
- [ ] **Day 2** — Read R02 and implement the SDK tool loop with `list_orders`. Record calls, arguments, results, stop reasons, and latency.

  **第 2 天** — 阅读 R02，用 SDK 实现 `list_orders` 工具循环，记录调用、参数、结果、停止原因和耗时。
- [ ] **Day 3** — Read R03. Add `check_refund_eligibility` and `submit_refund`. Specify schemas, success responses, and business errors.

  **第 3 天** — 阅读 R03，增加资格查询与退款工具，定义 schema、成功返回和业务错误。由程序验证身份、金额与确认状态。
- [ ] **Day 4** — Read R04. Implement multi-turn clarification and a centralized context builder. Inspect the context of each model call.

  **第 4 天** — 阅读 R04，实现多轮澄清和统一上下文组装，检查每次模型调用实际接收的内容。
- [ ] **Day 5** — Add bounded execution, tool timeouts, controlled retries, refund idempotency, and confirmation withdrawal. Exercise each failure.

  **第 5 天** — 加入执行预算、工具超时、有限重试、退款幂等和撤销确认，逐一触发异常。
- [ ] **Day 6** — Create 12 cases covering normal requests, ambiguity, invalid orders, permissions, confirmation, and failures. Change one factor and compare results.

  **第 6 天** — 建立 12 条样本，覆盖正常请求、歧义、无效订单、权限、确认和失败。只改变一个因素并比较结果。
- [ ] **Day 7** — Add three previously unseen cases. Demonstrate the agent, write a one-page design note, and record a three-minute English explanation.

  **第 7 天** — 新增三条未见样本，演示 Agent，写一页设计说明，并录制三分钟英文介绍。

### Acceptance Checklist

验收清单

- [ ] Explain the complete request–model–tool–result loop while locating each stage in the code.

  能解释完整调用循环，并在代码中指出对应位置。
- [ ] Show the final business state for every case and classify each failure. Correct permission, confirmation, and duplicate-submission failures before closing the week.

  展示每条样本的最终业务状态，分类记录失败，并修复权限、确认和重复提交相关问题后完成本周验收。
- [ ] Reproduce one failure and demonstrate that the fix also preserves the other checked cases.

  复现一个失败，展示修复效果并复查其他样本。
- [ ] Explain in English what the agent does, who enforces business rules, and one issue you fixed.

  能用英文说明 Agent 的功能、业务规则由谁校验，以及自己修复的一个问题。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Speak with approximately three reachable developers or individual users about their most recent attempt at a recurring task. Capture frequency, effort, existing tools, and sample inputs.

  尝试与约三位能接触到的开发者或个人用户交流，了解最近一次重复任务的过程，记录频率、投入、现有工具和输入样本。
- [ ] Select one task and write a one-page offer hypothesis naming the user, input, deliverable, benefit, and access channel. Adapt the engineering exercise to that task.

  选定一个任务，写一页产品假设，明确用户、输入、交付物、收益和接触渠道，并据此调整工程练习。
- [ ] Retain evidence of the problem and a concrete next step with a potential user. If evidence is weak, document the uncertainty and test another task.

  保留问题证据和与潜在用户约定的具体下一步。证据不足时记录不确定性并验证其他任务。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 2 — State, Memory, and Human Intervention

第 2 周 — 状态、记忆与人工介入

Study R06, prioritizing state, memory, streaming, and human intervention. Revisit R04 when designing context.

学习 R06，重点完成状态、记忆、流式响应和人工介入部分。设计上下文时回看 R04。

### Practice Checklist

练习清单

- [ ] Represent the existing agent with explicit graph state and documented transitions. Compare behavior with the Week 1 version.

  用明确的图状态和状态转换表达已有 Agent，与第 1 周版本比较行为。
- [ ] Persist conversations and isolate two users and two conversation threads.

  持久化会话，并验证两个用户、两个会话线程之间的隔离。
- [ ] Pause before refund submission, save the intended action, and resume after approval. Recheck ownership and eligibility on execution.

  退款前暂停并保存待执行操作，审批后恢复，执行时重新校验所有权与资格。
- [ ] Add streaming progress and document which information belongs in conversation state, durable memory, and business storage.

  增加流式进度反馈，说明会话状态、长期记忆和业务存储分别保存什么。

### Acceptance Checklist

验收清单

- [ ] Restart the process during an approval pause and successfully resume the intended task.

  在审批暂停时重启进程，能够恢复原任务。
- [ ] Demonstrate user and thread isolation with explicit assertions over stored state and tool access.

  通过对状态和工具访问的明确断言，验证用户与线程隔离。
- [ ] Run the Week 1 cases against the new implementation and investigate every behavioral change.

  对新实现运行第 1 周样本，分析每项行为变化。
- [ ] Explain checkpointing and external side effects separately, including the remaining failure window between them.

  分别解释 checkpoint 与外部副作用，以及两者之间仍存在的故障窗口。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Show the core workflow to potential users and observe them completing their own tasks. Record the baseline effort and assistance required.

  向潜在用户演示核心流程，观察他们完成自己的任务，记录原有投入和需要的人工协助。
- [ ] Define a small paid-pilot offer with deliverables, limits, price hypothesis, and support scope. Ask users to react to the offer.

  定义一个小规模付费试点方案，写清交付、限制、价格假设和支持范围，请用户给出反馈。
- [ ] Retain user-session evidence, a revised workflow, and a clear reason to continue or change the offer.

  保留用户操作证据、调整后的流程，以及继续或修改方案的明确理由。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 3 — Build a Trustworthy Evaluation Baseline

第 3 周 — 建立可信的评测基线

Study R07–R09. Allocate roughly three hours to course material and five to seven hours to implementation and review.

学习 R07–R09，约三小时用于课程资料，五至七小时用于实现和复核。

### Practice Checklist

练习清单

- [ ] Define task success, tool selection, argument accuracy, latency, cost, and confirmation compliance. Write down the denominators and scoring rules.

  定义任务成功、工具选择、参数准确、延迟、成本与确认合规指标，写明分母和评分规则。
- [ ] Expand the dataset to 50–100 cases with source and scenario labels. Separate development cases from a held-out set and freeze the first version.

  将数据集扩充到 50–100 条，记录来源和场景，区分开发集与保留集，并冻结首版数据。
- [ ] Build code-based checks for order ownership, refund amount, final state, and duplicate side effects.

  对订单所有权、退款金额、最终状态和重复副作用实现代码断言。
- [ ] Add one rubric-based LLM judge for an open-ended quality dimension. Compare its labels with human review and record disagreements.

  为一项开放质量指标增加带评分规则的 LLM Judge，与人工复核比较并记录分歧。
- [ ] Store per-case traces, versions, scores, and failure categories in a reproducible baseline report.

  保存逐例轨迹、版本、分数和失败分类，生成可复现的基线报告。

### Acceptance Checklist

验收清单

- [ ] Run the dataset from one documented command and report both aggregate metrics and scenario slices.

  通过一条有说明的命令运行数据集，同时输出总体指标和分场景结果。
- [ ] Verify that a fluent response claiming success fails when the business state is wrong.

  验证当业务状态错误时，声称成功的流畅回答会被判失败。
- [ ] Show examples of judge agreement and disagreement with human review, and describe the limits of the sample.

  展示 Judge 与人工一致及不一致的实例，并说明样本的局限。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Have target users review examples of acceptable and unacceptable results. Incorporate their criteria into the evaluation dataset and rubric.

  请目标用户判断可接受与不可接受结果，将他们的标准纳入评测集和评分规则。
- [ ] Measure useful outputs, correction time, and delivery effort on actual user tasks. Identify the minimum quality needed for a paid pilot.

  在实际用户任务上测量有效结果、修改时间与交付投入，明确付费试点需要的最低质量。
- [ ] Retain customer-grounded evaluation criteria and a baseline comparison with the current alternative.

  保留来源于用户的评测标准，以及与现有替代方式的基线比较。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 4 — Controlled Experiments and Regression Checks

第 4 周 — 对比实验与回归检查

Apply R08–R09. R10 provides optional practice in organizing experiments and rubrics.

应用 R08–R09，R10 可用于补充实验组织和评分规则练习。

### Practice Checklist

练习清单

- [ ] Pick two observed failure categories and form a testable hypothesis for each.

  选择两类已观察到的失败，各提出一个可验证假设。
- [ ] Run two experiments, changing one factor per experiment, such as tool descriptions or context selection. Compare on the same cases and environment.

  完成两次实验，每次改变一个因素，例如工具描述或上下文选择，使用同一组样本和环境比较。
- [ ] Repeat a representative subset to measure variation. Record run count, spread, and paired case-level changes.

  对代表性子集重复运行，记录运行次数、波动和同一案例的前后变化。
- [ ] Evaluate the final candidate on the held-out set. Define release checks from business risk and observed baseline behavior.

  在保留集上评估最终候选版本，依据业务风险和基线表现定义发布检查。
- [ ] Add automated regression runs and reports for changes to prompts, tools, models, and orchestration.

  为 Prompt、工具、模型和编排变化增加自动回归运行与报告。

### Acceptance Checklist

验收清单

- [ ] Explain why an apparent improvement is credible or inconclusive, including run variability and scenario regressions.

  结合运行波动与分场景回归，解释改善是否可信或仍无法判断。
- [ ] Deliberately introduce an incorrect refund amount and show that the regression check detects it.

  主动引入错误退款金额，展示回归检查能够发现。
- [ ] Produce a report that connects the hypothesis, code or configuration change, measurements, and decision.

  报告能够连接假设、代码或配置改动、测量结果与最终决策。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Offer the scoped paid pilot and record responses, objections, agreed terms, and payment status. Use a simple deployable workflow or assisted delivery to serve the pilot.

  提出范围明确的付费试点，记录反馈、异议、约定条款和付款状态，使用可部署的简单流程或辅助交付服务试点。
- [ ] Deliver the agreed result and record the model cost, manual corrections, turnaround time, and customer acceptance.

  交付约定结果，记录模型费用、人工修改、交付时间和客户验收。
- [ ] Retain actual payment and delivery evidence when achieved. Otherwise record the rejection reasons and the next experiment, with the payment goal pending.

  成交后保留真实付款与交付证据。尚未成交时记录拒绝原因和下一次实验，将付款目标保留为待完成。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 5 — Durable Execution and Side Effects

第 5 周 — 持久执行与副作用

Study R11 and begin R12's incident-response material. Build on the persistence implemented in Week 2.

学习 R11，并开始 R12 的事故处理内容，在第 2 周持久化实现上继续深入。

### Practice Checklist

练习清单

- [ ] Draw task, approval, and refund-operation state transitions. Identify each external write and its recovery behavior.

  绘制任务、审批和退款操作的状态转换，标明每个外部写入及恢复行为。
- [ ] Persist operation identifiers and use the same business idempotency key across retries and process restarts.

  持久化操作标识，在重试与进程重启后复用同一业务幂等键。
- [ ] Simulate a successful downstream refund followed by a lost response. Recover by checking the downstream operation status.

  模拟下游退款成功但响应丢失，通过查询下游操作状态恢复。
- [ ] Inject process termination before and after the external write and checkpoint. Exercise stale approvals and cancellation races.

  在外部写入和 checkpoint 前后注入进程终止，并练习过期审批和取消竞争。
- [ ] Define bounded retries, task deadlines, and an escalation or reconciliation path for uncertain outcomes.

  定义有限重试、任务截止时间，以及不确定结果的人工升级或对账路径。

### Acceptance Checklist

验收清单

- [ ] Show one refund record for each logical operation across the injected failure and retry cases.

  在故障和重试样本中，展示每个逻辑操作只对应一笔退款记录。
- [ ] Recover an interrupted task from persisted state and account for all external effects.

  从持久化状态恢复任务，并核对所有外部操作结果。
- [ ] Document the downstream assumptions, remaining consistency limits, and handling of unresolved operations.

  记录下游能力假设、剩余一致性限制和未决操作处理方式。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Agree with trial users on confirmation points, sensitive data access, failure handling, and support expectations for the selected task.

  与试用用户确认所选任务中的操作确认点、敏感数据访问、失败处理和支持预期。
- [ ] Observe another use of the product and measure how much founder intervention remains. Apply recovery work to the failures that affect delivery.

  观察用户再次使用产品，测量仍需多少个人介入，将恢复机制应用到影响交付的问题。
- [ ] Retain a support and recovery procedure plus a record of repeated use or the reason users stopped.

  保留支持与恢复流程，以及用户重复使用或停止使用的原因记录。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 6 — Observability, Performance, and Incident Response

第 6 周 — 可观测性、性能与事故处理

Complete R12's selected observability, cost/performance, and incident-response modules. Follow current framework documentation for API details.

完成 R12 的可观测性、成本性能和事故处理重点模块，具体 API 以当前框架文档为准。

### Practice Checklist

练习清单

- [ ] Propagate task and trace identifiers across model calls, tools, retries, and downstream services. Redact sensitive fields.

  在模型调用、工具、重试和下游服务间传递任务与追踪标识，并对敏感字段脱敏。
- [ ] Measure task success, tool errors, latency distribution, token usage, cost per successful task, and human escalation.

  测量任务成功、工具错误、延迟分布、token 用量、单次成功任务成本和人工升级情况。
- [ ] Exercise concurrent sessions, timeouts, and rate limits under a documented workload. Set provisional SLOs based on that workload and user needs.

  在有记录的负载下验证并发会话、超时和限流，结合负载与用户需求设置初步 SLO。
- [ ] Optimize one measured bottleneck, then rerun quality and permission checks to evaluate the trade-off.

  优化一个实际测量到的瓶颈，再运行质量与权限检查，分析取舍。
- [ ] Reproduce one incident from a saved trace and write its timeline, root cause, corrective action, and verification.

  从保存的轨迹复现一次事故，记录时间线、根因、修复和验证。

### Acceptance Checklist

验收清单

- [ ] Starting from a failed task identifier, locate the failing stage and relevant versions using the recorded telemetry.

  从失败任务标识出发，利用遥测定位失败阶段和相关版本。
- [ ] Compare baseline and optimized quality, latency, and cost under the same workload, including limitations.

  在同一负载下比较优化前后的质量、延迟和成本，并说明局限。
- [ ] Use the incident procedure to diagnose a second injected failure and record the recovery result.

  使用事故处理流程诊断第二个注入故障，并记录恢复结果。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Build a unit-cost sheet including successful tasks, failed attempts, retries, model and tool usage, hosting, payment fees, and support labor.

  建立单位成本表，计入成功任务、失败尝试、重试、模型工具使用、托管、支付手续费和支持人工。
- [ ] Compare pricing and usage limits with measured cost. Track acquisition spending and your time spent finding and serving users.

  用实测成本检查定价与用量限制，记录获客支出，以及寻找和服务用户的时间。
- [ ] Retain a period profit calculation and explain whether observed usage and pricing can sustain positive profit.

  保留周期利润核算，说明当前使用情况和定价是否能够维持正利润。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 7 — Cloud Deployment and Release Operations

第 7 周 — 云部署与发布运行

Choose R13A for AWS or R13B for Google Cloud. R14 is optional support for the Google route. If new platform setup exceeds this week's budget, document the remaining work and continue before checking cloud acceptance.

选择 AWS 路线 R13A 或 Google Cloud 路线 R13B，Google 路线可选学 R14。若新平台配置超出本周预算，记录剩余工作并继续完成后，再勾选云部署验收。

- [ ] AWS route selected / 已选择 AWS 路线
- [ ] Google Cloud route selected / 已选择 Google Cloud 路线

### Practice Checklist

练习清单

- [ ] Run the chosen official exercise, then deploy the study agent with persistent state and simulated business tools.

  完成所选官方练习，再部署自己的 Agent、持久化状态和模拟业务工具。
- [ ] Configure identity, credentials, service permissions, logs, tracing, resource limits, and a spending budget.

  配置身份、凭据、服务权限、日志、追踪、资源限制与费用预算。
- [ ] Run the frozen evaluation set against the deployed version and compare it with the local version.

  对云上版本运行冻结评测集，与本地版本比较。
- [ ] Publish a new version through a documented release procedure. Rehearse a rollback and verify existing task-state compatibility.

  按有记录的流程发布新版本，演练回滚并验证已有任务状态兼容性。
- [ ] Record provisioning and shutdown steps, observed costs, and how to reproduce the deployment.

  记录资源创建与关闭步骤、实际费用和部署复现方式。

### Acceptance Checklist

验收清单

- [ ] Complete one full approved refund flow in the cloud and identify its trace and final state.

  在云上完成一次经过确认的完整退款流程，找到对应轨迹与最终状态。
- [ ] Restart or redeploy a worker and demonstrate recovery using cloud-persisted state.

  重启或重新部署工作进程，展示通过云上持久化状态恢复。
- [ ] Show the rollback result, evaluation report, permission checks, and resource cleanup or continued-operation decision.

  展示回滚结果、评测报告、权限检查，以及资源清理或继续运行的决定。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Turn the pilot into a repeatable product workflow with onboarding, result delivery, support contact, and applicable payment or renewal handling.

  将试点整理为可重复交付的产品流程，补齐引导、结果交付、支持联系和适用的支付或续费处理。
- [ ] Invite another target user through a channel you can repeat. Record the path from first contact through use and purchase decision.

  通过可重复的渠道邀请另一位目标用户，记录首次接触、使用到购买决定的过程。
- [ ] Retain evidence of repeatable delivery and distinguish paid customers, active trials, and prospects.

  保留可重复交付的证据，分别记录付费客户、活跃试用者和潜在客户。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Week 8 — Consolidation and Interview Evidence

第 8 周 — 成果整合与面试表达

Review the earlier materials against the target role. Use the project evidence to identify gaps and complete the most relevant missing work.

对照目标岗位复查前面资料，使用项目证据识别缺口，并补齐最相关的工作。

### Practice Checklist

练习清单

- [ ] Prepare reproducible setup instructions, architecture and state diagrams, and tool contracts in English with Chinese translations where helpful.

  整理可复现的启动说明、架构与状态图、工具契约，使用英文并按需要补充中文翻译。
- [ ] Consolidate the evaluation baseline, two experiments, regression results, and dataset limitations.

  汇总评测基线、两次实验、回归结果和数据集局限。
- [ ] Consolidate fault-injection results, one incident review, performance measurements, and cloud deployment evidence.

  汇总故障注入、一次事故复盘、性能测量和云部署证据。
- [ ] Record a three-minute English project introduction and a ten-minute technical walkthrough. Practice follow-up questions on design, evaluation, and recovery.

  录制三分钟英文项目介绍和十分钟技术讲解，练习设计、评测与恢复方面的追问。
- [ ] Write resume bullets using measured results and distinguish personal implementation from framework and platform capabilities.

  根据实测结果写简历条目，讲清个人实现与框架、平台提供的能力。

### Acceptance Checklist

验收清单

- [ ] Reproduce the documented setup in a fresh environment and run the evaluation command successfully.

  在全新环境按文档启动项目，并成功运行评测命令。
- [ ] Explain one architectural choice, one measured quality improvement, and one production failure with evidence.

  能用证据解释一个架构选择、一次质量改善和一次生产故障。
- [ ] Complete an English mock interview, review the recording, and improve three unclear answers.

  完成一次英文模拟面试，复听录音并改进三个表达不清楚的回答。
- [ ] Record unresolved issues and the next study priorities based on the target job descriptions.

  记录未解决问题，并依据目标 JD 排出下一步学习重点。

### Commercial Practice and Evidence

商业实践与证据

- [ ] Review the full observation period, including revenue earned, refunds, operating costs, founder labor, repeat use, and outstanding customer obligations.

  复盘完整观察周期，核对已交付收入、退款、经营成本、个人工时、重复使用和未完成客户义务。
- [ ] Prepare a product demonstration and commercial case study alongside the engineering reports. Use actual numbers and identify estimates.

  在工程报告之外准备产品演示和商业案例，使用真实数字并标明估算。
- [ ] Check the commercial outcome items only when their evidence is available. Set the next iteration from customer and profitability results.

  商业目标有对应证据后再勾选，根据用户和利润结果确定下一轮迭代。

Completion date / 完成日期 — ____

Evidence link / 证据链接 — ____

Failures and next actions / 失败与后续行动 — ____

## Weekly Progress Tracker

每周进度记录

| Week / 周次 | Planned hours / 计划小时 | Actual hours / 实际小时 | Evidence / 证据 | Acceptance date / 验收日期 |
| --- | --- | --- | --- | --- |
| 1 | 10 | ____ | ____ | ____ |
| 2 | 8–10 | ____ | ____ | ____ |
| 3 | 8–10 | ____ | ____ | ____ |
| 4 | 8–10 | ____ | ____ | ____ |
| 5 | 8–10 | ____ | ____ | ____ |
| 6 | 8–10 | ____ | ____ | ____ |
| 7 | 8–10 | ____ | ____ | ____ |
| 8 | 8–10 | ____ | ____ | ____ |

## Resource Access and Version Notes

资料访问与版本说明

LangChain Academy currently describes its course content as free. DeepLearning.AI lists PRO access for graded assignments and certificates or accomplishments on the recommended courses. Cloud labs and model calls can incur charges. Check access and resource costs when starting an exercise. [LangChain Academy](https://academy.langchain.com/) · [Agentic AI](https://www.deeplearning.ai/courses/agentic-ai) · [Evaluating AI Agents](https://www.deeplearning.ai/courses/evaluating-ai-agents)

LangChain Academy 当前说明课程内容免费。推荐的 DeepLearning.AI 课程将评分作业、证书或完成凭证列为 PRO 权益。云实验和模型调用可能产生费用，开始练习时核对访问权益与资源费用。

Use engineering articles for architectural reasoning and current SDK documentation for executable examples. OpenAI's evaluation guide currently states that its Evals platform is being retired, with shutdown scheduled for November 30, 2026. Apply the evaluation methodology to your project's runner and verify current tooling before integrating a service. [OpenAI evaluation guide](https://developers.openai.com/api/docs/guides/evaluation-best-practices)

工程文章用于学习架构思路，可执行示例以当前 SDK 文档为准。OpenAI 评测指南当前注明其 Evals 平台正在退役，计划于 2026 年 11 月 30 日关闭。将评测方法应用到项目自己的运行器，接入服务前核对工具当前状态。
