# AI 工程师岗位要求、学习资料与 8 周计划

整理日期为 2026 年 11 月 19 日。

适用对象为具有中国国内 10 年软件开发经验，希望申请美国 Senior AI／Agent Engineer 岗位的工程师。学习重点包括 LLM 与 Agent 机制、系统化评测和生产可靠性，同时训练英文技术表达。

本文汇总此前的官方招聘 JD 与课程调研。岗位样本覆盖 Agent 应用、平台、企业交付和评测工程，采用定性比较。职位状态、课程目录和访问权益可能调整，申请或报名时以原始页面为准。文中的练习、验收方式和时间分配为学习建议。尚未实际跑完所列课程实验。

## 1. 岗位样本与方向

| 公司与岗位 | 美国地点 | 主要要求 | 官方 JD |
| --- | --- | --- | --- |
| OpenAI · Software Engineer, Agent Platform | 旧金山 | 大规模后端、分布式系统、Agent 执行编排、状态、资源管理、重试恢复、沙箱与运维 | [职位](https://openai.com/careers/software-engineer-agent-platform-san-francisco/) |
| OpenAI · Applied AI Engineer, Enterprise | 旧金山／纽约 | Python、生产 AI 系统、评测、企业集成、质量与成本取舍，以及客户技术沟通 | [职位](https://openai.com/careers/applied-ai-engineer-enterprise-san-francisco/) |
| Anthropic · Staff+ Software Engineer, Claude Managed Agents | 旧金山／纽约 | 至少 8 年相关工程经验，长任务、持久化、沙箱、上下文、记忆、Agent 执行循环及评测 | [职位](https://job-boards.greenhouse.io/anthropic/jobs/5395767008) |
| Anthropic · Staff Software Engineer, GTM AI Engineering | 旧金山／西雅图 | Python 或 TypeScript、SQL、生产 LLM、MCP、会话分析、评测、审批与业务效果衡量 | [职位](https://job-boards.greenhouse.io/anthropic/jobs/5390966008-51) |
| Google DeepMind · Staff Software Engineer | 山景城／纽约 | 大型生产系统与架构经验，分布式评测执行引擎、Agent 循环、工具调用、LLM Judge、错误分类及 SLO | [职位](https://www.google.com/about/careers/applications/jobs/results/124548522136478406-staff-software-engineer/) |
| Google DeepMind · Staff Research Scientist/Engineer, Consumer Agents Post Training | 美国多地 | 8 年软件经验、LLM、强化学习与深度学习，Agent 后训练、个性化、实验和数据构建 | [职位](https://www.google.com/about/careers/applications/jobs/results/120683810973983430-staff-research-scientistengineer-consumer-agents-post-training-deepmind) |
| Microsoft AI · Software Engineer, Model API Infra | 山景城／雷德蒙德 | 5 年以上工程经验或等效经历，分布式服务、API、部署自动化、Kubernetes，模型与 Agent 服务经验为加分项 | [职位](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4438720009) |
| Microsoft AI · Software Engineer, Health Evaluations | 纽约 | 6 年以上工程经验、跨团队领导、多轮仿真、轨迹评测、自动评分与专家标注校准 | [职位](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4391533009) |
| AWS · Software Development Engineer, AgentCore | 纽约 | 3 年以上开发、2 年以上设计／架构，运行时、会话隔离、权限、工具编排与可靠性 | [职位](https://www.amazon.jobs/en/jobs/10565536/software-development-engineer-agentcore-aws-agentic-ai) |
| 6sense · Senior AI Engineer, Agentic Platform | 湾区／奥斯汀 | 5 年以上生产软件、2 年以上生产 LLM，Python、LangGraph 或同类框架、MCP、检索、评测与多租户系统 | [职位](https://job-boards.greenhouse.io/6sense/jobs/8257108) |
| HeyGen · Applied AI Engineer, Video Agent | 旧金山／帕洛阿尔托／洛杉矶 | 真实用户使用的 Agent、多步规划、工具调用、失败恢复、评测，Python、TypeScript 与 React | [职位](https://job-boards.greenhouse.io/heygen/jobs/5255664007) |
| Scale AI · Senior Frontier Agents Engineer, Applied AI | 旧金山 | 5 年以上相关经验，Python、生产 LLM、检索、记忆、工具使用、定量评测与客户合作 | [职位](https://job-boards.greenhouse.io/scaleai/jobs/4720478005) |
| Scale AI · Senior Frontier Agents Engineer, Forward Deployed Engineering | 旧金山 | 5 年以上软件经验，Python、分布式系统、云部署、企业 API 集成、监控和故障恢复 | [职位](https://job-boards.greenhouse.io/scaleai/jobs/4694863005) |
| Rocket Money · Staff Applied AI Engineer | 美国多地／美国境内远程 | Agent 共享能力平台、工具执行、授权、评测、追踪、恢复及跨团队技术影响力 | [职位](https://job-boards.greenhouse.io/truebill/jobs/8004786003) |

各岗位职级不同，差异同时受到团队任务与职级影响。Senior、Staff、Staff+ 需要分别对照个人责任范围和跨团队影响力。职位支持搬迁、申请表询问担保需求时，仍需与招聘方确认是否接受海外新工签申请。

此前发现的 DeepMind Applied AI Agents, Professional Intelligence 和 Agent Data Quality 页面打开后显示 Job not found，本文岗位表采用可打开详情的其他样本。

## 2. 共性能力

| 能力 | 具体要求 | 应准备的证据 |
| --- | --- | --- |
| 软件工程 | 熟练编程、API、数据存储、测试、系统设计与调试 | 生产代码、架构取舍、规模和线上问题 |
| LLM 与 Agent | 工具调用、编排、状态、上下文、检索和记忆 | 完整执行链路与设计依据 |
| 系统化评测 | 数据集、评分规则、回归、实验、人工校准与失败分析 | 评测报告和改进前后对比 |
| 可靠性 | 超时、重试、幂等、恢复、监控和发布 | 故障实验与事故复盘 |
| 安全边界 | 授权、租户隔离、工具权限、审批和审计 | 权限模型和边界测试 |
| 性能与成本 | 质量、延迟、吞吐、模型及调用费用的权衡 | 测量数据与优化决策 |
| 端到端交付 | 澄清需求、实施、上线、运行和跨团队沟通 | 个人贡献及业务结果 |

上述要求反复出现在平台、应用和企业交付岗位中。模型训练、强化学习与深层推理优化需要根据目标方向进一步深入。[OpenAI 平台 JD](https://openai.com/careers/software-engineer-agent-platform-san-francisco/) · [Anthropic 平台 JD](https://job-boards.greenhouse.io/anthropic/jobs/5395767008) · [微软模型平台 JD](https://job-boards.greenhouse.io/microsoftcorporation/jobs/4438720009)

## 3. 三个核心方向的具体要求

### 3.1 理解 LLM 与 Agent 工作机制

| 主题 | 应掌握的深度 |
| --- | --- |
| 模型调用 | Token、上下文窗口、采样、结构化输出、流式响应、工具调用，分别验证格式、参数和业务正确性 |
| 执行循环 | 实现模型调用、工具请求、参数校验、执行、结果回传与结束，设计停止条件和预算 |
| 编排选择 | 根据任务选择固定工作流、路由、单 Agent、多 Agent，并验证收益及新增失败点 |
| 上下文 | 管理指令、历史、工具结果和检索内容，处理截断、摘要、压缩及过期信息 |
| 工具契约 | 名称、描述、schema、错误语义、鉴权、分页、重复调用及结果长度 |
| 检索与记忆 | 区分会话状态、长期记忆和外部知识，排查召回、重排、权限过滤及引用错误 |

建议能够用一条业务执行链路说明状态在哪里保存、控制流由谁决定、工具怎样授权、何时请求澄清、何时结束。[Agent 架构](https://www.anthropic.com/research/building-effective-agents) · [上下文工程](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents) · [工具设计](https://www.anthropic.com/research/writing-tools-for-agents)

自测问题包括以下内容。

- 为什么为这个任务选择当前编排，替代方案的效果和成本如何？
- 工具选对了但参数错了，如何定位到上下文、描述或参数生成？
- 长会话中用户约束丢失，怎样定位并验证修复？
- 如何证明记忆或多 Agent 设计带来了可测量的收益？

### 3.2 系统化评测能力

| 层次 | 评测内容 |
| --- | --- |
| 任务结果 | 目标是否完成，最终业务状态、约束和交付物是否正确 |
| 执行过程 | 意图、工具选择、参数、工具结果利用和执行步骤 |
| 回答质量 | 准确性、完整性、依据与引用支持程度 |
| 安全边界 | 越权、数据泄漏、审批绕过和不允许的操作 |
| 效率体验 | 延迟、步骤数、调用次数、成功任务成本和人工接管率 |

应能建设从数据到发布的评测闭环。

1. 收集有代表性的数据，覆盖高频任务、边界、多轮、历史失败、权限和工具异常。
2. 明确成功条件与评分标准，保留独立测试集和数据版本。
3. 对可精确验证的结果写程序断言，对开放结果采用明确 rubric 的模型评分，并与人工标注校准。
4. 控制实验变量，记录模型、Prompt、工具、数据和配置版本，对随机性进行重复测量。
5. 按场景和失败原因分析变化，连接回归、发布检查和线上抽样。

学习时重点关注最终业务状态、逐步执行质量和评分器可信度。[微软 Agent 评测](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators?view=foundry-classic) · [Anthropic 评测指南](https://www.anthropic.com/research/demystifying-evals-for-ai-agents) · [OpenAI 评测最佳实践](https://developers.openai.com/api/docs/guides/evaluation-best-practices)

自测问题包括以下内容。

- 成功率从 80% 升到 85%，如何判断改善可信？
- Judge 与人工意见不一致，怎样检查评分规则和数据？
- 离线指标提高但线上投诉增加，怎样设计排查和验证？
- 模型升级前，哪些任务和指标需要达到业务定义的发布要求？

### 3.3 生产可靠性

| 场景 | 应具备的设计能力 |
| --- | --- |
| 超时、429、服务故障 | 单次及任务总超时、重试预算、退避、限流、并发控制和降级 |
| 外部操作结果未知 | 幂等键、操作记录、结果查询、对账与人工处理 |
| 长任务进程终止 | 状态持久化、checkpoint、恢复位置和版本兼容 |
| 重复或错误行动 | 循环检测、预算、业务校验和人工接管 |
| 审批期间数据变化 | 保存待审批操作，恢复时重新验证必要条件 |
| 多租户与权限 | 服务端授权、隔离、凭据管理和关键操作审计 |
| 模型及工具升级 | 版本追踪、回归、灰度和回滚 |
| 排障 | 关联任务、步骤、模型、配置、工具状态、重试、耗时、token 和费用，控制敏感数据访问 |

典型问题是退款实际成功、响应返回前超时，随后进程崩溃。需要协调业务幂等、下游结果查询、checkpoint 与外部事务边界，以及无法确认时的对账流程。[LangGraph 持久化](https://docs.langchain.com/oss/python/langgraph/persistence) · [故障容错](https://docs.langchain.com/oss/python/langgraph/fault-tolerance) · [人工中断](https://docs.langchain.com/oss/python/langgraph/interrupts)

## 4. 课程与学习资料

筛选优先考虑大厂官方资料，并补充框架作者课程和成熟教学平台的专项课。口碑判断主要依据讲师背景、平台成熟度与实践内容，本次未取得统一口径的独立课程评分。

### 4.1 Agent 机制与编排

| 优先级 | 资源与提供方 | 学习重点 | 时长或形式 |
| --- | --- | --- | --- |
| 主线 | [Building effective agents · Anthropic](https://www.anthropic.com/research/building-effective-agents) | 工作流、路由、规划、工具和架构选择 | 官方工程文章 |
| 主线 | [Writing effective tools for agents · Anthropic](https://www.anthropic.com/research/writing-tools-for-agents) | 工具契约、返回值与评测 | 官方工程文章 |
| 主线 | [Effective context engineering · Anthropic](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents) | 上下文、信息取舍、摘要与记忆 | 官方工程文章 |
| 主线 | [Introduction to LangGraph — Python · LangChain Academy](https://academy.langchain.com/courses/intro-to-langgraph) | 状态、记忆、流式执行、人工介入、子图和部署 | 官方标注约 6 小时视频，免费 |
| 可选 | [Agentic AI · Andrew Ng／DeepLearning.AI](https://www.deeplearning.ai/courses/agentic-ai) | 系统学习工具使用、反思、规划、多 Agent、评测及错误分析 | 官方标注约 7 小时 45 分钟 |
| 快速补充 | [AI Agents in LangGraph · DeepLearning.AI／LangChain／Tavily](https://www.deeplearning.ai/courses/ai-agents-in-langgraph) | 从原生 Agent 到 LangGraph，持久化、流式执行与人工介入 | 官方标注约 1 小时 32 分钟 |

LangChain 和 DeepLearning.AI 属于补充来源。优先完成主线，视频偏好者可选 Andrew Ng 课程。学习代码时对照当前 SDK 文档核对版本。

### 4.2 系统化评测

| 优先级 | 资源与提供方 | 学习重点 | 时长或形式 |
| --- | --- | --- | --- |
| 主线课程 | [Evaluating AI Agents · DeepLearning.AI／Arize AI](https://www.deeplearning.ai/courses/evaluating-ai-agents) | Tracing、组件与端到端评测、代码评分、LLM Judge、实验 | 官方标注约 2 小时 16 分钟 |
| 主线阅读 | [Demystifying evals for AI agents · Anthropic](https://www.anthropic.com/research/demystifying-evals-for-ai-agents) | 任务、轨迹、评分器、随机性与回归 | 官方工程文章 |
| 主线阅读 | [Evaluation best practices · OpenAI](https://developers.openai.com/api/docs/guides/evaluation-best-practices) | 目标、数据、指标、版本比较、人工校准与持续评测 | 官方文档 |
| 主线模块 | [Evaluate and optimize AI agents through structured experiments · Microsoft Learn](https://learn.microsoft.com/en-us/training/modules/evaluate-optimize-agents/) | Git 实验组织、rubric、质量、成本和性能比较 | 官方标注约 1 小时 6 分钟 |
| 参考 | [Agent evaluators · Microsoft Learn](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators?view=foundry-classic) | 任务完成、工具选择、参数与执行质量的指标设计 | 官方文档 |

### 4.3 可靠性、运维与云部署

| 优先级 | 资源与提供方 | 学习重点 |
| --- | --- | --- |
| 主线 | [LangGraph Persistence](https://docs.langchain.com/oss/python/langgraph/persistence)、[Fault tolerance](https://docs.langchain.com/oss/python/langgraph/fault-tolerance)、[Interrupts](https://docs.langchain.com/oss/python/langgraph/interrupts) | 持久化、恢复、人工暂停与执行语义 |
| 主线选读 | [Monitor, evaluate, and operate multi-agent AI solutions in Azure · Microsoft Learn](https://learn.microsoft.com/en-us/training/paths/aaai-4-monitor-evaluate-operate-multi-agent-ai-solutions-azure/) | 五个高级模块，涵盖 OpenTelemetry、评测、成本性能、人工审批和事故处理 |
| AWS 实践 | [Getting started with AgentCore · AWS](https://catalog.workshops.aws/agentcore-getting-started/en-US) | 运行时、记忆、工具、认证、可观测性、评测与治理 |
| Google 实践 | [Build and Deploy Agents in Production · Google Skills](https://www.skills.google/paths/3802/course_templates/1633) | ADK 架构与 Cloud Run／GKE 部署入门，官方标注约 45 分钟 |
| Google 工程参考 | [Agent Starter Pack · Google Cloud](https://github.com/GoogleCloudPlatform/agent-starter-pack) | 带 CI/CD、评测与可观测性的部署模板 |

## 5. 8 周学习计划

每周预计投入 8–10 小时，总计约 64–80 小时。前提是能够使用 Python 完成基本服务与脚本开发，能够使用 Git 和常见部署工具。若 Python 熟练度不足，增加热身时间。每周建议约三成时间学习、六成编码与实验、一成英文表达。

建议贯穿一个熟悉业务的项目，例如订单售后 Agent。用合成数据和可控测试工具模拟订单查询、政策检索、退款申请与审批。各阶段持续完善同一个系统。

| 周次 | 学习安排 | 实践交付 | 自测验收 |
| --- | --- | --- | --- |
| 第 1 周 | 精读 Anthropic 三篇机制文章，可选 Andrew Ng 视频对应章节 | 用原生 SDK 写工具调用循环，定义查询和操作工具、停止条件、执行预算与日志 | 能解释完整请求链路、控制流、工具契约与上下文取舍 |
| 第 2 周 | LangChain Academy，重点状态与记忆、人工介入 | 持久化、流式执行、审批、状态恢复，并对比原生实现与框架实现 | 暂停后能继续，能够解释恢复时的重执行及外部副作用 |
| 第 3 周 | Evaluating AI Agents 和微软实验模块 | 首版 50–100 条样本、程序断言、rubric、人工复核和基线报告 | 区分任务成功、工具正确和回答质量，能解释数据覆盖 |
| 第 4 周 | Anthropic 与 OpenAI 评测指南，重复实验与失败分析 | 对工具描述和上下文等做两次受控改动，形成版本对比、重复运行结果和失败分类 | 能说明改善是否可信、哪些场景回归，以及如何决定是否发布 |
| 第 5 周 | LangGraph 持久化、故障容错与人工中断文档 | 幂等、结果查询、任务恢复、超时、重试预算和循环检测，执行故障注入 | 外部操作成功但响应丢失时，恢复流程能避免重复操作 |
| 第 6 周 | 微软高级路径中的可观测性、成本性能、故障诊断 | 端到端 Tracing、指标、敏感字段处理、发布回归和一份故障复盘 | 可由任务 ID 定位到具体失败步骤，并解释恢复和修复验证 |
| 第 7 周 | 根据已有经验选择 AWS 或 Google 实践 | 云部署、身份权限、监控、版本发布与资源清理流程 | 能演示端到端任务，定位失败，解释资源与模型调用成本 |
| 第 8 周 | 对照目标 JD 查漏补缺，集中英文演练 | 英文架构说明、评测报告、事故复盘和演示，说明个人贡献 | 10 分钟英文讲解，再接受机制、评测、恢复、权限、延迟和成本追问 |

50–100 条样本用于首版练习，正式发布所需的数据覆盖、风险阈值和测试规模应由具体业务决定。每阶段以完成交付和能够解释设计为进度依据。

## 6. 最终成果与面试表达

建议项目成果包含以下内容。

- 可运行的 Agent 与可控工具环境，附启动、配置和演示说明。
- 架构说明，覆盖状态、上下文、工具、权限、停止与恢复机制。
- 评测集说明、评分规则、基线和改进对比，标明数据与版本。
- 失败分类和一次质量改善记录。
- 一次故障注入或生产事故复盘，包含触发、影响、定位、修复与验证。
- 英文项目讲解，说明个人负责范围、主要取舍和可核验结果。

每周练习以下英文问题，并用自己的真实项目回答。

1. How does your agent decide which tool to call and when to stop?
2. How do you manage context and state across a long-running task?
3. How do you know that a change actually improved the agent?
4. How do you calibrate an LLM judge against human judgments?
5. What happens if a tool succeeds but its response is lost?
6. How do you diagnose a failure across the model, tools, and downstream services?
7. What did you personally own, and what trade-off did you make?

针对平台岗，重点展示运行时、状态、恢复和规模。针对应用岗，重点展示工具、上下文、评测和用户效果。针对企业交付岗，补充需求澄清、客户系统集成和英文方案沟通。

## 7. 资源状态与使用说明

- LangChain Academy 说明课程内容免费。DeepLearning.AI 的部分作业和证书涉及 PRO，具体访问权益以课程页面为准。[LangChain Academy](https://academy.langchain.com/) · [DeepLearning.AI](https://www.deeplearning.ai/courses/agentic-ai)
- 云实验、模型 API 与托管服务可能产生费用，创建资源前检查当前价格，实验后清理资源。
- 截至本次调研，OpenAI 评测指南标注 Evals 平台自 2026 年 10 月 31 日只读，计划于 11 月 30 日关闭。本文使用该指南学习评测方法，实践需根据当前产品文档选择实现方式。[官方说明](https://developers.openai.com/api/docs/guides/evaluation-best-practices)
- Anthropic 旧课程仓库已归档，其内容含较早模型与 SDK 示例。本文主线采用工程文章与当前框架文档。[旧课程仓库状态](https://github.com/anthropics/courses)
- 部分课程详情页和 Workshop 需要登录或 JavaScript，本次核查依据可访问官方内容及官方搜索索引，尚未验证所有账号、地区和付费权限。
