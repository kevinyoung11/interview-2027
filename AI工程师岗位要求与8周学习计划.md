# AI Engineer Job Requirements, Learning Resources, and an Eight-Week Plan

AI 工程师岗位要求、学习资料与 8 周计划

Prepared on November 19, 2026.

整理日期为 2026 年 11 月 19 日。

This guide is for a software engineer with 10 years of development experience in China who plans to apply for Senior AI or Agent Engineer roles in the United States. It focuses on LLM and agent mechanisms, systematic evaluation, and production reliability, alongside technical communication in English.

适用对象为具有中国国内 10 年软件开发经验，希望申请美国 Senior AI／Agent Engineer 岗位的工程师。学习重点包括 LLM 与 Agent 机制、系统化评测和生产可靠性，同时训练英文技术表达。

This document brings together the earlier research on official job descriptions and courses. It compares selected roles in agent applications, platforms, enterprise delivery, and evaluation engineering qualitatively. Job availability, course curricula, and access terms can change, so check the original pages when applying or enrolling. Exercises, acceptance criteria, and time allocations are study recommendations. The listed course labs have yet to be completed in practice.

本文汇总此前的官方招聘 JD 与课程调研。岗位样本覆盖 Agent 应用、平台、企业交付和评测工程，采用定性比较。职位状态、课程目录和访问权益可能调整，申请或报名时以原始页面为准。文中的练习、验收方式和时间分配为学习建议。尚未实际跑完所列课程实验。

## 1. Representative Roles and Career Directions

**岗位样本与方向**

| Company and role<br>公司与岗位 | U.S. location<br>美国地点 | Key requirements<br>主要要求 | Official job description<br>官方 JD |
| --- | --- | --- | --- |
| OpenAI · Software Engineer, Agent Platform<br>OpenAI · Agent 平台软件工程师 | San Francisco<br>旧金山 | Large-scale backend and distributed systems, agent execution and orchestration, state, resource management, retries, recovery, sandboxing, and operations<br>大规模后端、分布式系统、Agent 执行编排、状态、资源管理、重试恢复、沙箱与运维 | [Job description](https://openai.com/careers/software-engineer-agent-platform-san-francisco/)<br>[职位](https://openai.com/careers/software-engineer-agent-platform-san-francisco/) |
| OpenAI · Applied AI Engineer, Enterprise<br>OpenAI · 企业应用 AI 工程师 | San Francisco / New York<br>旧金山／纽约 | Python, production AI systems, evaluations, enterprise integration, quality and cost trade-offs, and customer technical communication<br>Python、生产 AI 系统、评测、企业集成、质量与成本取舍，以及客户技术沟通 | [Job description](https://openai.com/careers/applied-ai-engineer-enterprise-san-francisco/)<br>[职位](https://openai.com/careers/applied-ai-engineer-enterprise-san-francisco/) |
| Anthropic · Staff+ Software Engineer, Claude Managed Agents<br>Anthropic · Claude 托管 Agent 平台 Staff+ 软件工程师 | San Francisco / New York<br>旧金山／纽约 | At least 8 years of relevant engineering experience, long-running tasks, persistence, sandboxing, context, memory, agent loops, and evaluations<br>至少 8 年相关工程经验，长任务、持久化、沙箱、上下文、记忆、Agent 执行循环及评测 | [Job description](https://job-boards.greenhouse.io/anthropic/jobs/5395767008)<br>[职位](https://job-boards.greenhouse.io/anthropic/jobs/5395767008) |
| Anthropic · Staff Software Engineer, GTM AI Engineering<br>Anthropic · 市场与销售 AI 工程 Staff 软件工程师 | San Francisco / Seattle<br>旧金山／西雅图 | Python or TypeScript, SQL, production LLM systems, MCP, transcript analysis, evaluations, approvals, and business outcome measurement<br>Python 或 TypeScript、SQL、生产 LLM、MCP、会话分析、评测、审批与业务效果衡量 | [Job description](https://job-boards.greenhouse.io/anthropic/jobs/5390966008-51)<br>[职位](https://job-boards.greenhouse.io/anthropic/jobs/5390966008-51) |
| Google DeepMind · Staff Software Engineer<br>Google DeepMind · Staff 软件工程师 | Mountain View / New York<br>山景城／纽约 | Large production systems and architecture, distributed evaluation execution, agent loops, tool use, LLM judges, error classification, and SLOs<br>大型生产系统与架构经验，分布式评测执行引擎、Agent 循环、工具调用、LLM Judge、错误分类及 SLO | [Job description](https://www.google.com/about/careers/applications/jobs/results/124548522136478406-staff-software-engineer/)<br>[职位](https://www.google.com/about/careers/applications/jobs/results/124548522136478406-staff-software-engineer/) |
| Google DeepMind · Staff Research Scientist/Engineer, Consumer Agents Post Training<br>Google DeepMind · 消费者 Agent 后训练 Staff 研究科学家／工程师 | Multiple U.S. locations<br>美国多地 | 8 years of software experience, LLMs, reinforcement learning and deep learning, agent post-training, personalization, experiments, and dataset development<br>8 年软件经验、LLM、强化学习与深度学习，Agent 后训练、个性化、实验和数据构建 | [Job description](https://www.google.com/about/careers/applications/jobs/results/120683810973983430-staff-research-scientistengineer-consumer-agents-post-training-deepmind)<br>[职位](https://www.google.com/about/careers/applications/jobs/results/120683810973983430-staff-research-scientistengineer-consumer-agents-post-training-deepmind) |
| Microsoft AI · Software Engineer, Model API Infra<br>Microsoft AI · 模型 API 基础设施软件工程师 | Mountain View / Redmond<br>山景城／雷德蒙德 | 5+ years of engineering experience or equivalent, distributed services, APIs, deployment automation, and Kubernetes. Model and agent serving experience is a plus<br>5 年以上工程经验或等效经历，分布式服务、API、部署自动化、Kubernetes，模型与 Agent 服务经验为加分项 | [Job description](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4438720009)<br>[职位](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4438720009) |
| Microsoft AI · Software Engineer, Health Evaluations<br>Microsoft AI · 医疗评测软件工程师 | New York<br>纽约 | 6+ years of engineering experience, cross-functional leadership, multi-turn simulation, trajectory evaluation, and calibration of automated grading against expert annotations<br>6 年以上工程经验、跨团队领导、多轮仿真、轨迹评测、自动评分与专家标注校准 | [Job description](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4391533009)<br>[职位](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4391533009) |
| AWS · Software Development Engineer, AgentCore<br>AWS · AgentCore 软件开发工程师 | New York<br>纽约 | 3+ years of development and 2+ years of design or architecture, runtimes, session isolation, permissions, tool orchestration, and reliability<br>3 年以上开发、2 年以上设计／架构，运行时、会话隔离、权限、工具编排与可靠性 | [Job description](https://www.amazon.jobs/en/jobs/10565536/software-development-engineer-agentcore-aws-agentic-ai)<br>[职位](https://www.amazon.jobs/en/jobs/10565536/software-development-engineer-agentcore-aws-agentic-ai) |
| 6sense · Senior AI Engineer, Agentic Platform<br>6sense · Agent 平台资深 AI 工程师 | Bay Area / Austin<br>湾区／奥斯汀 | 5+ years of production software and 2+ years of production LLM systems, Python, LangGraph or comparable frameworks, MCP, retrieval, evaluation, and multi-tenant systems<br>5 年以上生产软件、2 年以上生产 LLM，Python、LangGraph 或同类框架、MCP、检索、评测与多租户系统 | [Job description](https://job-boards.greenhouse.io/6sense/jobs/8257108)<br>[职位](https://job-boards.greenhouse.io/6sense/jobs/8257108) |
| HeyGen · Applied AI Engineer, Video Agent<br>HeyGen · 视频 Agent 应用 AI 工程师 | San Francisco / Palo Alto / Los Angeles<br>旧金山／帕洛阿尔托／洛杉矶 | Agents used by real users, multi-step planning, tool use, failure recovery, evaluations, Python, TypeScript, and React<br>真实用户使用的 Agent、多步规划、工具调用、失败恢复、评测，Python、TypeScript 与 React | [Job description](https://job-boards.greenhouse.io/heygen/jobs/5255664007)<br>[职位](https://job-boards.greenhouse.io/heygen/jobs/5255664007) |
| Scale AI · Senior Frontier Agents Engineer, Applied AI<br>Scale AI · 应用 AI 方向资深前沿 Agent 工程师 | San Francisco<br>旧金山 | 5+ years of relevant experience, Python, production LLM systems, retrieval, memory, tool use, quantitative evaluation, and customer collaboration<br>5 年以上相关经验，Python、生产 LLM、检索、记忆、工具使用、定量评测与客户合作 | [Job description](https://job-boards.greenhouse.io/scaleai/jobs/4720478005)<br>[职位](https://job-boards.greenhouse.io/scaleai/jobs/4720478005) |
| Scale AI · Senior Frontier Agents Engineer, Forward Deployed Engineering<br>Scale AI · 前线部署方向资深前沿 Agent 工程师 | San Francisco<br>旧金山 | 5+ years of software experience, Python, distributed systems, cloud deployment, enterprise API integration, monitoring, and failure recovery<br>5 年以上软件经验，Python、分布式系统、云部署、企业 API 集成、监控和故障恢复 | [Job description](https://job-boards.greenhouse.io/scaleai/jobs/4694863005)<br>[职位](https://job-boards.greenhouse.io/scaleai/jobs/4694863005) |
| Rocket Money · Staff Applied AI Engineer<br>Rocket Money · Staff 应用 AI 工程师 | Multiple U.S. locations / U.S. remote<br>美国多地／美国境内远程 | Shared agent capabilities, tool execution, authorization, evaluation, tracing, recovery, and technical influence across teams<br>Agent 共享能力平台、工具执行、授权、评测、追踪、恢复及跨团队技术影响力 | [Job description](https://job-boards.greenhouse.io/truebill/jobs/8004786003)<br>[职位](https://job-boards.greenhouse.io/truebill/jobs/8004786003) |

The roles span different levels, and their requirements reflect both team responsibilities and seniority. Assess Senior, Staff, and Staff+ roles against your scope of ownership and influence across teams. If a posting offers relocation or asks about sponsorship, confirm with the recruiter whether the team supports new work visa applications for candidates based overseas.

各岗位职级不同，差异同时受到团队任务与职级影响。Senior、Staff、Staff+ 需要分别对照个人责任范围和跨团队影响力。职位支持搬迁、申请表询问担保需求时，仍需与招聘方确认是否接受海外新工签申请。

The previously identified DeepMind Applied AI Agents, Professional Intelligence and Agent Data Quality pages displayed “Job not found” when opened. The table uses other samples whose job details were accessible.

此前发现的 DeepMind Applied AI Agents, Professional Intelligence 和 Agent Data Quality 页面打开后显示 Job not found，本文岗位表采用可打开详情的其他样本。

## 2. Shared Competencies

**共性能力**

| Competency<br>能力 | Specific requirements<br>具体要求 | Evidence to prepare<br>应准备的证据 |
| --- | --- | --- |
| Software engineering<br>软件工程 | Programming, APIs, storage, testing, system design, and debugging<br>熟练编程、API、数据存储、测试、系统设计与调试 | Production code, architectural trade-offs, scale, and operational issues<br>生产代码、架构取舍、规模和线上问题 |
| LLMs and agents<br>LLM 与 Agent | Tool use, orchestration, state, context, retrieval, and memory<br>工具调用、编排、状态、上下文、检索和记忆 | A complete execution trace and design rationale<br>完整执行链路与设计依据 |
| Systematic evaluation<br>系统化评测 | Datasets, rubrics, regression tests, experiments, human calibration, and failure analysis<br>数据集、评分规则、回归、实验、人工校准与失败分析 | Evaluation reports and before-and-after comparisons<br>评测报告和改进前后对比 |
| Reliability<br>可靠性 | Timeouts, retries, idempotency, recovery, monitoring, and releases<br>超时、重试、幂等、恢复、监控和发布 | Fault experiments and incident reviews<br>故障实验与事故复盘 |
| Security boundaries<br>安全边界 | Authorization, tenant isolation, tool permissions, approvals, and auditing<br>授权、租户隔离、工具权限、审批和审计 | Permission models and boundary tests<br>权限模型和边界测试 |
| Performance and cost<br>性能与成本 | Trade-offs among quality, latency, throughput, models, and API costs<br>质量、延迟、吞吐、模型及调用费用的权衡 | Measurements and optimization decisions<br>测量数据与优化决策 |
| End-to-end delivery<br>端到端交付 | Requirements clarification, implementation, release, operations, and cross-functional communication<br>澄清需求、实施、上线、运行和跨团队沟通 | Personal contributions and business outcomes<br>个人贡献及业务结果 |

These requirements recur across platform, application, and enterprise delivery roles. Model training, reinforcement learning, and advanced inference optimization require further depth according to your target specialization. [OpenAI platform JD](https://openai.com/careers/software-engineer-agent-platform-san-francisco/) · [Anthropic platform JD](https://job-boards.greenhouse.io/anthropic/jobs/5395767008) · [Microsoft model platform JD](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4438720009)

上述要求反复出现在平台、应用和企业交付岗位中。模型训练、强化学习与深层推理优化需要根据目标方向进一步深入。[OpenAI 平台 JD](https://openai.com/careers/software-engineer-agent-platform-san-francisco/) · [Anthropic 平台 JD](https://job-boards.greenhouse.io/anthropic/jobs/5395767008) · [微软模型平台 JD](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4438720009)

## 3. Detailed Requirements in Three Core Areas

**三个核心方向的具体要求**

### 3.1 Understanding LLM and Agent Mechanisms

**理解 LLM 与 Agent 工作机制**

| Topic<br>主题 | Expected depth<br>应掌握的深度 |
| --- | --- |
| Model invocation<br>模型调用 | Tokens, context windows, sampling, structured output, streaming, and tool calling. Validate format, arguments, and business correctness separately<br>Token、上下文窗口、采样、结构化输出、流式响应、工具调用，分别验证格式、参数和业务正确性 |
| Agent execution loop<br>执行循环 | Implement model calls, tool requests, argument validation, execution, result feedback, and termination. Define stopping conditions and budgets<br>实现模型调用、工具请求、参数校验、执行、结果回传与结束，设计停止条件和预算 |
| Orchestration choices<br>编排选择 | Choose fixed workflows, routing, single agents, or multiple agents according to the task. Verify benefits and additional failure modes<br>根据任务选择固定工作流、路由、单 Agent、多 Agent，并验证收益及新增失败点 |
| Context management<br>上下文 | Manage instructions, history, tool results, and retrieved content. Handle truncation, summarization, compaction, and stale information<br>管理指令、历史、工具结果和检索内容，处理截断、摘要、压缩及过期信息 |
| Tool contracts<br>工具契约 | Names, descriptions, schemas, error semantics, authentication, pagination, duplicate calls, and response length<br>名称、描述、schema、错误语义、鉴权、分页、重复调用及结果长度 |
| Retrieval and memory<br>检索与记忆 | Distinguish session state, long-term memory, and external knowledge. Diagnose recall, reranking, permission filtering, and citation errors<br>区分会话状态、长期记忆和外部知识，排查召回、重排、权限过滤及引用错误 |

Be able to explain a complete business workflow, including where state is stored, what determines control flow, how tools are authorized, when clarification is requested, and when execution ends. [Agent architecture](https://www.anthropic.com/research/building-effective-agents) · [Context engineering](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents) · [Tool design](https://www.anthropic.com/research/writing-tools-for-agents)

建议能够用一条业务执行链路说明状态在哪里保存、控制流由谁决定、工具怎样授权、何时请求澄清、何时结束。[Agent 架构](https://www.anthropic.com/research/building-effective-agents) · [上下文工程](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents) · [工具设计](https://www.anthropic.com/research/writing-tools-for-agents)

Use the following questions to assess your understanding.

自测问题包括以下内容。

- Why did you choose this orchestration approach, and how do alternatives compare in effectiveness and cost?<br>
  为什么为这个任务选择当前编排，替代方案的效果和成本如何？
- If the agent selects the correct tool but supplies incorrect arguments, how do you trace the issue to context, tool descriptions, or argument generation?<br>
  工具选对了但参数错了，如何定位到上下文、描述或参数生成？
- If user constraints are lost during a long conversation, how do you diagnose the cause and validate a fix?<br>
  长会话中用户约束丢失，怎样定位并验证修复？
- How do you demonstrate a measurable benefit from memory or a multi-agent design?<br>
  如何证明记忆或多 Agent 设计带来了可测量的收益？

### 3.2 Systematic Evaluation

**系统化评测能力**

| Level<br>层次 | What to evaluate<br>评测内容 |
| --- | --- |
| Task outcome<br>任务结果 | Goal completion and correctness of final business state, constraints, and deliverables<br>目标是否完成，最终业务状态、约束和交付物是否正确 |
| Execution process<br>执行过程 | Intent, tool selection, arguments, use of tool results, and execution steps<br>意图、工具选择、参数、工具结果利用和执行步骤 |
| Response quality<br>回答质量 | Accuracy, completeness, grounding, and citation support<br>准确性、完整性、依据与引用支持程度 |
| Security boundaries<br>安全边界 | Unauthorized access, data leakage, approval bypasses, and prohibited actions<br>越权、数据泄漏、审批绕过和不允许的操作 |
| Efficiency and experience<br>效率体验 | Latency, step count, invocation count, cost per successful task, and human takeover rate<br>延迟、步骤数、调用次数、成功任务成本和人工接管率 |

Be able to build an evaluation feedback loop from data collection through release.

应能建设从数据到发布的评测闭环。

1. Collect representative data covering frequent tasks, boundary cases, multi-turn interactions, historical failures, permissions, and tool errors.<br>
   收集有代表性的数据，覆盖高频任务、边界、多轮、历史失败、权限和工具异常。
2. Define success conditions and grading criteria, and maintain an independent test set and dataset versions.<br>
   明确成功条件与评分标准，保留独立测试集和数据版本。
3. Use programmatic assertions for precisely verifiable outcomes. For open-ended outcomes, use model graders with explicit rubrics and calibrate them against human annotations.<br>
   对可精确验证的结果写程序断言，对开放结果采用明确 rubric 的模型评分，并与人工标注校准。
4. Control experimental variables, record model, prompt, tool, data, and configuration versions, and repeat runs to measure variability.<br>
   控制实验变量，记录模型、Prompt、工具、数据和配置版本，对随机性进行重复测量。
5. Analyze changes by scenario and failure cause, and connect findings to regression tests, release checks, and production sampling.<br>
   按场景和失败原因分析变化，连接回归、发布检查和线上抽样。

Focus on final business state, execution quality at each step, and the trustworthiness of graders. [Microsoft agent evaluation](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators?view=foundry-classic) · [Anthropic evaluation guide](https://www.anthropic.com/research/demystifying-evals-for-ai-agents) · [OpenAI evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices)

学习时重点关注最终业务状态、逐步执行质量和评分器可信度。[微软 Agent 评测](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators?view=foundry-classic) · [Anthropic 评测指南](https://www.anthropic.com/research/demystifying-evals-for-ai-agents) · [OpenAI 评测最佳实践](https://developers.openai.com/api/docs/guides/evaluation-best-practices)

Use the following questions to assess your understanding.

自测问题包括以下内容。

- If success rises from 80% to 85%, how do you establish that the improvement is credible?<br>
  成功率从 80% 升到 85%，如何判断改善可信？
- If a judge disagrees with human reviewers, how do you inspect the rubric and data?<br>
  Judge 与人工意见不一致，怎样检查评分规则和数据？
- If offline metrics improve while production complaints increase, how do you investigate and validate your findings?<br>
  离线指标提高但线上投诉增加，怎样设计排查和验证？
- Before upgrading a model, which tasks and metrics must meet business-defined release criteria?<br>
  模型升级前，哪些任务和指标需要达到业务定义的发布要求？

### 3.3 Production Reliability

**生产可靠性**

| Scenario<br>场景 | Expected design capability<br>应具备的设计能力 |
| --- | --- |
| Timeouts, HTTP 429, and service failures<br>超时、429、服务故障 | Per-call and total task timeouts, retry budgets, backoff, rate limits, concurrency control, and fallback behavior<br>单次及任务总超时、重试预算、退避、限流、并发控制和降级 |
| Unknown external operation outcome<br>外部操作结果未知 | Idempotency keys, operation records, status queries, reconciliation, and human resolution<br>幂等键、操作记录、结果查询、对账与人工处理 |
| Process termination during a long task<br>长任务进程终止 | Persistent state, checkpoints, recovery positions, and version compatibility<br>状态持久化、checkpoint、恢复位置和版本兼容 |
| Repeated or incorrect actions<br>重复或错误行动 | Loop detection, budgets, business validation, and human takeover<br>循环检测、预算、业务校验和人工接管 |
| Data changes while awaiting approval<br>审批期间数据变化 | Persist the pending operation and revalidate necessary conditions when execution resumes<br>保存待审批操作，恢复时重新验证必要条件 |
| Multiple tenants and permissions<br>多租户与权限 | Server-side authorization, isolation, credential management, and critical-operation audits<br>服务端授权、隔离、凭据管理和关键操作审计 |
| Model and tool upgrades<br>模型及工具升级 | Version tracking, regression checks, gradual rollout, and rollback<br>版本追踪、回归、灰度和回滚 |
| Debugging<br>排障 | Correlate tasks, steps, models, configurations, tool status, retries, duration, tokens, and costs. Control access to sensitive data<br>关联任务、步骤、模型、配置、工具状态、重试、耗时、token 和费用，控制敏感数据访问 |

Consider a refund that succeeds, followed by a timeout before the response arrives and then a process crash. You need to coordinate business idempotency, downstream status queries, checkpoint boundaries, external transactions, and reconciliation when the outcome cannot be confirmed. [LangGraph persistence](https://docs.langchain.com/oss/python/langgraph/persistence) · [Fault tolerance](https://docs.langchain.com/oss/python/langgraph/fault-tolerance) · [Interrupts](https://docs.langchain.com/oss/python/langgraph/interrupts)

典型问题是退款实际成功、响应返回前超时，随后进程崩溃。需要协调业务幂等、下游结果查询、checkpoint 与外部事务边界，以及无法确认时的对账流程。[LangGraph 持久化](https://docs.langchain.com/oss/python/langgraph/persistence) · [故障容错](https://docs.langchain.com/oss/python/langgraph/fault-tolerance) · [人工中断](https://docs.langchain.com/oss/python/langgraph/interrupts)

## 4. Courses and Learning Resources

**课程与学习资料**

The selection prioritizes official resources from major technology companies, supplemented by courses from framework authors and established teaching platforms. Reputation was assessed mainly through instructor backgrounds, platform maturity, and practical content. Comparable independent course ratings were unavailable in this research.

筛选优先考虑大厂官方资料，并补充框架作者课程和成熟教学平台的专项课。口碑判断主要依据讲师背景、平台成熟度与实践内容，本次未取得统一口径的独立课程评分。

### 4.1 Agent Mechanisms and Orchestration

**Agent 机制与编排**

| Priority<br>优先级 | Resource and provider<br>资源与提供方 | Learning focus<br>学习重点 | Duration or format<br>时长或形式 |
| --- | --- | --- | --- |
| Core<br>主线 | [Building effective agents · Anthropic](https://www.anthropic.com/research/building-effective-agents)<br>[构建高效 Agent · Anthropic](https://www.anthropic.com/research/building-effective-agents) | Workflows, routing, planning, tools, and architecture choices<br>工作流、路由、规划、工具和架构选择 | Official engineering article<br>官方工程文章 |
| Core<br>主线 | [Writing effective tools for agents · Anthropic](https://www.anthropic.com/research/writing-tools-for-agents)<br>[为 Agent 设计高效工具 · Anthropic](https://www.anthropic.com/research/writing-tools-for-agents) | Tool contracts, return values, and evaluation<br>工具契约、返回值与评测 | Official engineering article<br>官方工程文章 |
| Core<br>主线 | [Effective context engineering · Anthropic](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents)<br>[高效上下文工程 · Anthropic](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents) | Context, information selection, summarization, and memory<br>上下文、信息取舍、摘要与记忆 | Official engineering article<br>官方工程文章 |
| Core<br>主线 | [Introduction to LangGraph — Python · LangChain Academy](https://academy.langchain.com/courses/intro-to-langgraph)<br>[LangGraph 入门，Python 版 · LangChain Academy](https://academy.langchain.com/courses/intro-to-langgraph) | State, memory, streaming, human intervention, subgraphs, and deployment<br>状态、记忆、流式执行、人工介入、子图和部署 | Approximately 6 hours of video, free according to the provider<br>官方标注约 6 小时视频，免费 |
| Optional<br>可选 | [Agentic AI · Andrew Ng/DeepLearning.AI](https://www.deeplearning.ai/courses/agentic-ai)<br>[Agentic AI，智能体 AI · 吴恩达／DeepLearning.AI](https://www.deeplearning.ai/courses/agentic-ai) | Tool use, reflection, planning, multiple agents, evaluation, and error analysis<br>系统学习工具使用、反思、规划、多 Agent、评测及错误分析 | Approximately 7 hours 45 minutes according to the provider<br>官方标注约 7 小时 45 分钟 |
| Quick supplement<br>快速补充 | [AI Agents in LangGraph · DeepLearning.AI/LangChain/Tavily](https://www.deeplearning.ai/courses/ai-agents-in-langgraph)<br>[使用 LangGraph 构建 AI Agent · DeepLearning.AI／LangChain／Tavily](https://www.deeplearning.ai/courses/ai-agents-in-langgraph) | From a custom agent to LangGraph, persistence, streaming, and human intervention<br>从原生 Agent 到 LangGraph，持久化、流式执行与人工介入 | Approximately 1 hour 32 minutes according to the provider<br>官方标注约 1 小时 32 分钟 |

LangChain and DeepLearning.AI provide supplementary resources. Complete the core resources first. If you prefer video instruction, consider Andrew Ng’s course. Check current SDK documentation when working through code examples.

LangChain 和 DeepLearning.AI 属于补充来源。优先完成主线，视频偏好者可选 Andrew Ng 课程。学习代码时对照当前 SDK 文档核对版本。

### 4.2 Systematic Evaluation

**系统化评测**

| Priority<br>优先级 | Resource and provider<br>资源与提供方 | Learning focus<br>学习重点 | Duration or format<br>时长或形式 |
| --- | --- | --- | --- |
| Core course<br>主线课程 | [Evaluating AI Agents · DeepLearning.AI/Arize AI](https://www.deeplearning.ai/courses/evaluating-ai-agents)<br>[评测 AI Agent · DeepLearning.AI／Arize AI](https://www.deeplearning.ai/courses/evaluating-ai-agents) | Tracing, component and end-to-end evaluations, code graders, LLM judges, and experiments<br>Tracing、组件与端到端评测、代码评分、LLM Judge、实验 | Approximately 2 hours 16 minutes according to the provider<br>官方标注约 2 小时 16 分钟 |
| Core reading<br>主线阅读 | [Demystifying evals for AI agents · Anthropic](https://www.anthropic.com/research/demystifying-evals-for-ai-agents)<br>[理解 AI Agent 评测 · Anthropic](https://www.anthropic.com/research/demystifying-evals-for-ai-agents) | Tasks, trajectories, graders, variability, and regression<br>任务、轨迹、评分器、随机性与回归 | Official engineering article<br>官方工程文章 |
| Core reading<br>主线阅读 | [Evaluation best practices · OpenAI](https://developers.openai.com/api/docs/guides/evaluation-best-practices)<br>[评测最佳实践 · OpenAI](https://developers.openai.com/api/docs/guides/evaluation-best-practices) | Objectives, data, metrics, version comparisons, human calibration, and continuous evaluation<br>目标、数据、指标、版本比较、人工校准与持续评测 | Official documentation<br>官方文档 |
| Core module<br>主线模块 | [Evaluate and optimize AI agents through structured experiments · Microsoft Learn](https://learn.microsoft.com/en-us/training/modules/evaluate-optimize-agents/)<br>[通过结构化实验评测和优化 AI Agent · 微软学习平台](https://learn.microsoft.com/en-us/training/modules/evaluate-optimize-agents/) | Git-based experiments, rubrics, quality, cost, and performance comparisons<br>Git 实验组织、rubric、质量、成本和性能比较 | Approximately 1 hour 6 minutes according to the provider<br>官方标注约 1 小时 6 分钟 |
| Reference<br>参考 | [Agent evaluators · Microsoft Learn](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators?view=foundry-classic)<br>[Agent 评测器 · 微软学习平台](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators?view=foundry-classic) | Metric design for task completion, tool selection, arguments, and execution quality<br>任务完成、工具选择、参数与执行质量的指标设计 | Official documentation<br>官方文档 |

### 4.3 Reliability, Operations, and Cloud Deployment

**可靠性、运维与云部署**

| Priority<br>优先级 | Resource and provider<br>资源与提供方 | Learning focus<br>学习重点 |
| --- | --- | --- |
| Core<br>主线 | [LangGraph Persistence](https://docs.langchain.com/oss/python/langgraph/persistence), [Fault tolerance](https://docs.langchain.com/oss/python/langgraph/fault-tolerance), [Interrupts](https://docs.langchain.com/oss/python/langgraph/interrupts)<br>[LangGraph 持久化](https://docs.langchain.com/oss/python/langgraph/persistence)、[故障容错](https://docs.langchain.com/oss/python/langgraph/fault-tolerance)、[人工中断](https://docs.langchain.com/oss/python/langgraph/interrupts) | Persistence, recovery, human pauses, and execution semantics<br>持久化、恢复、人工暂停与执行语义 |
| Selected core reading<br>主线选读 | [Monitor, evaluate, and operate multi-agent AI solutions in Azure · Microsoft Learn](https://learn.microsoft.com/en-us/training/paths/aaai-4-monitor-evaluate-operate-multi-agent-ai-solutions-azure/)<br>[在 Azure 中监控、评测和运维多 Agent AI 解决方案 · 微软学习平台](https://learn.microsoft.com/en-us/training/paths/aaai-4-monitor-evaluate-operate-multi-agent-ai-solutions-azure/) | Five advanced modules covering OpenTelemetry, evaluation, cost and performance, human approvals, and incident response<br>五个高级模块，涵盖 OpenTelemetry、评测、成本性能、人工审批和事故处理 |
| AWS practice<br>AWS 实践 | [Getting started with AgentCore · AWS](https://catalog.workshops.aws/agentcore-getting-started/en-US)<br>[AgentCore 入门 · AWS](https://catalog.workshops.aws/agentcore-getting-started/en-US) | Runtimes, memory, tools, authentication, observability, evaluation, and governance<br>运行时、记忆、工具、认证、可观测性、评测与治理 |
| Google practice<br>Google 实践 | [Build and Deploy Agents in Production · Google Skills](https://www.skills.google/paths/3802/course_templates/1633)<br>[在生产环境构建和部署 Agent · Google Skills](https://www.skills.google/paths/3802/course_templates/1633) | ADK architecture and introductory deployment on Cloud Run or GKE. Approximately 45 minutes according to the provider<br>ADK 架构与 Cloud Run／GKE 部署入门，官方标注约 45 分钟 |
| Google engineering reference<br>Google 工程参考 | [Agent Starter Pack · Google Cloud](https://github.com/GoogleCloudPlatform/agent-starter-pack)<br>[Agent 工程启动模板 · Google Cloud](https://github.com/GoogleCloudPlatform/agent-starter-pack) | Deployment templates with CI/CD, evaluation, and observability<br>带 CI/CD、评测与可观测性的部署模板 |

## 5. The Eight-Week Study Plan

**8 周学习计划**

Plan for 8–10 hours per week, or approximately 64–80 hours in total. This assumes you can build basic services and scripts in Python and use Git and common deployment tools. Add preparation time if your Python skills need work. Allocate roughly 30% of each week to study, 60% to coding and experiments, and 10% to explaining technical work in English.

每周预计投入 8–10 小时，总计约 64–80 小时。前提是能够使用 Python 完成基本服务与脚本开发，能够使用 Git 和常见部署工具。若 Python 熟练度不足，增加热身时间。每周建议约三成时间学习、六成编码与实验、一成英文表达。

Use one project in a familiar business domain throughout the plan, such as an order support agent. Use synthetic data and controlled test tools to simulate order queries, policy retrieval, refund requests, and approvals. Improve the same system in each phase.

建议贯穿一个熟悉业务的项目，例如订单售后 Agent。用合成数据和可控测试工具模拟订单查询、政策检索、退款申请与审批。各阶段持续完善同一个系统。

| Week<br>周次 | Study activities<br>学习安排 | Practical deliverables<br>实践交付 | Acceptance criteria<br>自测验收 |
| --- | --- | --- | --- |
| Week 1<br>第 1 周 | Study Anthropic’s three mechanism articles. Optionally watch the corresponding Andrew Ng lessons<br>精读 Anthropic 三篇机制文章，可选 Andrew Ng 视频对应章节 | Build a tool-calling loop with a model SDK. Define query and action tools, stopping conditions, execution budgets, and logs<br>用原生 SDK 写工具调用循环，定义查询和操作工具、停止条件、执行预算与日志 | Explain the complete request lifecycle, control flow, tool contracts, and context choices<br>能解释完整请求链路、控制流、工具契约与上下文取舍 |
| Week 2<br>第 2 周 | Study LangChain Academy, focusing on state, memory, and human intervention<br>LangChain Academy，重点状态与记忆、人工介入 | Add persistence, streaming, approvals, and state recovery. Compare custom and framework-based implementations<br>持久化、流式执行、审批、状态恢复，并对比原生实现与框架实现 | Resume after a pause and explain re-execution and external side effects during recovery<br>暂停后能继续，能够解释恢复时的重执行及外部副作用 |
| Week 3<br>第 3 周 | Take Evaluating AI Agents and Microsoft’s experimentation module<br>Evaluating AI Agents 和微软实验模块 | Create an initial 50–100 cases, programmatic assertions, rubrics, human review, and a baseline report<br>首版 50–100 条样本、程序断言、rubric、人工复核和基线报告 | Distinguish task success, tool correctness, and response quality, and explain dataset coverage<br>区分任务成功、工具正确和回答质量，能解释数据覆盖 |
| Week 4<br>第 4 周 | Read Anthropic and OpenAI evaluation guides. Practice repeated experiments and failure analysis<br>Anthropic 与 OpenAI 评测指南，重复实验与失败分析 | Make two controlled changes to tool descriptions, context, or similar components. Record version comparisons, repeated runs, and failure categories<br>对工具描述和上下文等做两次受控改动，形成版本对比、重复运行结果和失败分类 | Explain the credibility of improvements, identify regressions, and justify release decisions<br>能说明改善是否可信、哪些场景回归，以及如何决定是否发布 |
| Week 5<br>第 5 周 | Study LangGraph persistence, fault tolerance, and interrupts<br>LangGraph 持久化、故障容错与人工中断文档 | Implement idempotency, status queries, task recovery, timeouts, retry budgets, and loop detection. Inject failures<br>幂等、结果查询、任务恢复、超时、重试预算和循环检测，执行故障注入 | Recover after a successful external operation with a lost response while avoiding duplicate actions<br>外部操作成功但响应丢失时，恢复流程能避免重复操作 |
| Week 6<br>第 6 周 | Study observability, cost and performance, and incident diagnosis in Microsoft’s advanced path<br>微软高级路径中的可观测性、成本性能、故障诊断 | Add end-to-end tracing, metrics, sensitive-field handling, release regression checks, and an incident review<br>端到端 Tracing、指标、敏感字段处理、发布回归和一份故障复盘 | Use a task ID to locate a failed step and explain recovery, the fix, and verification<br>可由任务 ID 定位到具体失败步骤，并解释恢复和修复验证 |
| Week 7<br>第 7 周 | Choose AWS or Google practice based on prior experience<br>根据已有经验选择 AWS 或 Google 实践 | Deploy to the cloud and implement identity, permissions, monitoring, versioned releases, and resource cleanup<br>云部署、身份权限、监控、版本发布与资源清理流程 | Demonstrate an end-to-end task, diagnose a failure, and explain resource and model invocation costs<br>能演示端到端任务，定位失败，解释资源与模型调用成本 |
| Week 8<br>第 8 周 | Review target job descriptions and practice technical communication in English<br>对照目标 JD 查漏补缺，集中英文演练 | Prepare an English architecture explanation, evaluation report, incident review, and demonstration showing personal ownership<br>英文架构说明、评测报告、事故复盘和演示，说明个人贡献 | Deliver a 10-minute presentation in English and answer follow-ups on mechanisms, evaluation, recovery, permissions, latency, and cost<br>10 分钟英文讲解，再接受机制、评测、恢复、权限、延迟和成本追问 |

Use 50–100 cases for the initial exercise. Determine production data coverage, risk thresholds, and test scale according to the business. Advance through each phase when you can demonstrate the deliverables and explain the design.

50–100 条样本用于首版练习，正式发布所需的数据覆盖、风险阈值和测试规模应由具体业务决定。每阶段以完成交付和能够解释设计为进度依据。

## 6. Final Deliverables and Interview Communication

**最终成果与面试表达**

Aim to produce the following project artifacts.

建议项目成果包含以下内容。

- A runnable agent and controlled tool environment, with setup, configuration, and demonstration instructions.<br>
  可运行的 Agent 与可控工具环境，附启动、配置和演示说明。
- An architecture explanation covering state, context, tools, permissions, stopping conditions, and recovery.<br>
  架构说明，覆盖状态、上下文、工具、权限、停止与恢复机制。
- Dataset documentation, grading criteria, baselines, and improvement comparisons with data and version identifiers.<br>
  评测集说明、评分规则、基线和改进对比，标明数据与版本。
- A failure taxonomy and a record of one quality improvement.<br>
  失败分类和一次质量改善记录。
- A fault-injection or production incident review covering the trigger, impact, investigation, fix, and verification.<br>
  一次故障注入或生产事故复盘，包含触发、影响、定位、修复与验证。
- An English project presentation explaining your personal ownership, major trade-offs, and verifiable results.<br>
  英文项目讲解，说明个人负责范围、主要取舍和可核验结果。

Practice the following English questions each week using your own real projects.

每周练习以下英文问题，并用自己的真实项目回答。

1. How does your agent decide which tool to call and when to stop?<br>
   你的 Agent 如何决定调用哪个工具，以及何时停止？
2. How do you manage context and state across a long-running task?<br>
   你如何管理长任务中的上下文和状态？
3. How do you know that a change actually improved the agent?<br>
   你如何判断一次改动确实改善了 Agent？
4. How do you calibrate an LLM judge against human judgments?<br>
   你如何用人工判断校准 LLM 评分器？
5. What happens if a tool succeeds but its response is lost?<br>
   工具执行成功但响应丢失时，会发生什么？
6. How do you diagnose a failure across the model, tools, and downstream services?<br>
   你如何跨模型、工具和下游服务诊断故障？
7. What did you personally own, and what trade-off did you make?<br>
   你个人负责了什么，做过什么取舍？

For platform roles, emphasize runtimes, state, recovery, and scale. For application roles, emphasize tools, context, evaluation, and user outcomes. For enterprise delivery roles, also demonstrate requirements clarification, customer system integration, and technical discussions in English.

针对平台岗，重点展示运行时、状态、恢复和规模。针对应用岗，重点展示工具、上下文、评测和用户效果。针对企业交付岗，补充需求澄清、客户系统集成和英文方案沟通。

## 7. Resource Availability and Usage Notes

**资源状态与使用说明**

- LangChain Academy states that course content is free. Some DeepLearning.AI assignments and certificates require PRO. Check the course pages for current access terms. [LangChain Academy](https://academy.langchain.com/) · [DeepLearning.AI](https://www.deeplearning.ai/courses/agentic-ai)<br>
  LangChain Academy 说明课程内容免费。DeepLearning.AI 的部分作业和证书涉及 PRO，具体访问权益以课程页面为准。[LangChain Academy](https://academy.langchain.com/) · [DeepLearning.AI](https://www.deeplearning.ai/courses/agentic-ai)
- Cloud labs, model APIs, and hosted services may incur charges. Check current pricing before provisioning resources and clean up after experiments.<br>
  云实验、模型 API 与托管服务可能产生费用，创建资源前检查当前价格，实验后清理资源。
- At the time of this research, OpenAI’s evaluation guide stated that the Evals platform became read-only on October 31, 2026, with shutdown scheduled for November 30. Use the guide for evaluation methodology and consult current product documentation when choosing an implementation. [Official documentation](https://developers.openai.com/api/docs/guides/evaluation-best-practices)<br>
  截至本次调研，OpenAI 评测指南标注 Evals 平台自 2026 年 10 月 31 日只读，计划于 11 月 30 日关闭。本文使用该指南学习评测方法，实践需根据当前产品文档选择实现方式。[官方说明](https://developers.openai.com/api/docs/guides/evaluation-best-practices)
- Anthropic’s older course repository is archived and contains examples using earlier models and SDKs. The core resources in this guide use engineering articles and current framework documentation. [Archived course repository](https://github.com/anthropics/courses)<br>
  Anthropic 旧课程仓库已归档，其内容含较早模型与 SDK 示例。本文主线采用工程文章与当前框架文档。[旧课程仓库状态](https://github.com/anthropics/courses)
- Some course pages and workshops require sign-in or JavaScript. This review relied on accessible official content and official search-index results. Account, regional, and paid access have yet to be fully verified.<br>
  部分课程详情页和 Workshop 需要登录或 JavaScript，本次核查依据可访问官方内容及官方搜索索引，尚未验证所有账号、地区和付费权限。
