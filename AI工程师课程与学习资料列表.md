# AI Engineer Courses and Learning Resources

AI 工程师课程与学习资料列表

Prepared on November 19, 2026, for a software engineer with 10 years of development experience preparing for Senior AI / Agent Engineer roles.

整理于 2026 年 11 月 19 日，适用于具有 10 年开发经验、准备申请 Senior AI／Agent Engineer 岗位的工程师。

Use the courses to deliver a complete AI product for developers or individual users, with real payment, repeat-use evidence, and positive operating profit. Study in the order shown below, moving from LLM and agent mechanisms to systematic evaluation and production reliability. Required and optional labels reflect the recommended eight-week plan. The course labs have yet to be run as part of preparing these documents.

通过课程完成面向开发者或个人用户的完整 AI 产品，验证真实付款、重复使用与正向经营利润。按下列顺序学习，从 LLM 与 Agent 机制进入系统化评测，再进入生产可靠性。必学、选学标记对应推荐的八周计划。整理文档时尚未实际运行课程实验。

For weekly exercises and acceptance criteria, use the [eight-week study checklist](AI工程师8周学习打卡清单.md). The [companion guide](AI工程师岗位要求与8周学习计划.md) provides job requirements and background research.

每周练习与验收标准见[八周学习打卡清单](AI工程师8周学习打卡清单.md)，岗位要求与背景调研见[配套指南](AI工程师岗位要求与8周学习计划.md)。

## Learning Order and Priorities

学习顺序与优先级

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

## Resource Access and Version Notes

资料访问与版本说明

LangChain Academy currently describes its course content as free. DeepLearning.AI lists PRO access for graded assignments and certificates or accomplishments on the recommended courses. Cloud labs and model calls can incur charges. Check access and resource costs when starting an exercise. [LangChain Academy](https://academy.langchain.com/) · [Agentic AI](https://www.deeplearning.ai/courses/agentic-ai) · [Evaluating AI Agents](https://www.deeplearning.ai/courses/evaluating-ai-agents)

LangChain Academy 当前说明课程内容免费。推荐的 DeepLearning.AI 课程将评分作业、证书或完成凭证列为 PRO 权益。云实验和模型调用可能产生费用，开始练习时核对访问权益与资源费用。

Use engineering articles for architectural reasoning and current SDK documentation for executable examples. OpenAI's evaluation guide currently states that its Evals platform is being retired, with shutdown scheduled for November 30, 2026. Apply the evaluation methodology to your project's runner and verify current tooling before integrating a service. [OpenAI evaluation guide](https://developers.openai.com/api/docs/guides/evaluation-best-practices)

工程文章用于学习架构思路，可执行示例以当前 SDK 文档为准。OpenAI 评测指南当前注明其 Evals 平台正在退役，计划于 2026 年 11 月 30 日关闭。将评测方法应用到项目自己的运行器，接入服务前核对工具当前状态。
