# 02 · 工程师转 Agent / AI Infra

适合有编程基础,想从传统SDE转向AI Infra、大模型训练、Agent开发方向的人。建议按下面顺序看。

## 入门顺位

### Stanford CS336 · Language Modeling from Scratch
- 2025版playlist:https://www.youtube.com/playlist?list=PLoROMvodv4rOY23Y0BoGoBGgQ1zmU_MT_
- 2026版playlist:https://www.youtube.com/playlist?list=PLoROMvodv4rMqXOcazWaTUHhq-yembLCV
- 中文摘要:从零手写一个语言模型,覆盖数据处理、Tokenization、Transformer架构、训练、并行、推理、评测全流程。目前公认转LLM工程方向最扎实的一门课,业内讨论"转型AI Infra看这个就够"通常指的就是它。
- 已知讲座(按标题,非精确时间戳):Lecture 1 Overview & Tokenization / Lecture 3 Architectures / Lecture 10 Inference,完整列表见playlist
- 📝 [Lecture 1 详细时间戳笔记](./notes/cs336-lecture1.md)——已整理
- ⚠️ 这门课还有个"Stanford Online"付费高管教育版本(10周,7875美金,含员工支持和作业批改),我们这里链的是免费YouTube录像,只有录像没有支持和批改,这是免费版本的取舍,别搞混两个版本

### Stanford CS230 · Deep Learning
- playlist:https://www.youtube.com/playlist?list=PLoROMvodv4rOABXSygHTsbvUz4G_YQhOb
- 中文摘要:深度学习基础,CNN/RNN/优化方法,给CS336打地基用

### Stanford CS224N · NLP with Deep Learning
- playlist:https://www.youtube.com/playlist?list=PLoROMvodv4rOhcuXMZkNm7j3fVwBBY42z
- 中文摘要:NLP+深度学习专项,词向量、Attention、Transformer在NLP场景的具体应用

### 补充基础(可选)
- CS229 机器学习:https://www.youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU
- CS234 强化学习:https://www.youtube.com/playlist?list=PLoROMvodv4rOSOPzutgyCTapiGlY2Nd8u

## 进阶:已有基础,想追前沿Agent/RL研究

### Georgia Tech CS8803 · Large Language Models(2026春季)
- 官方课程页(含完整课表):https://cocoxu.github.io/CS8803-LLM-spring2026/
- 主讲:Wei Xu
- 中文摘要:本质是一份"2026大模型前沿论文精读清单",逐周主题+对应论文如下(已核实,来自官方课程表):

| 时间 | 主题 | 代表论文 |
|---|---|---|
| Jan 12 | 课程总览 | 如何读论文 |
| Feb 2 | 预训练 | Chameleon数据混合框架、Parity-Aware BPE |
| Feb 4-9 | 表示学习/Embedding | LLM改进文本嵌入、MMTEB、DeepSeek-V2 §2.1、NV-Embed |
| Feb 11 | 混合专家(MoE) | Sparsely-Gated MoE、MoE作为嵌入模型 |
| Feb 16-18 | 推理与对齐 | BIRD贝叶斯推理框架、DPO直接偏好优化 |
| Feb 23 | Agent Harness | Agent Workflow Memory、OpenHands Software Agent SDK |
| Feb 25 | 长上下文 | Attention Sinks流式推理 |
| Mar 2 | 注意力机制 | DeepSeek-V3.2 §2、TransMLA |
| Mar 4 | 强化学习 | GRPO、DAPO、R1-Zero-Like训练 |
| Mar 9-11 | 推理系统 | Optimas复合AI系统优化、CWM代码生成世界模型 |
| Mar 16-18 | 自博弈RL | Absolute Zero、SPICE、SWE-RL |
| Mar 30 | 测试时扩展 | Learning to Discover、Test-Time Compute Scaling |
| Apr 1 | 模型同质化 | Artificial Hivemind |
| Apr 6 | 线性Transformer | Fast Weight Programmers、Delta Rule并行化 |
| Apr 8 | 扩散语言模型 | Diffusion-LM可控生成、大规模语言扩散模型 |
| Apr 13-15 | 安全与可解释性 | 涌现性错位对齐、稀疏自编码器/交叉编码器 |
| Apr 20-22 | 校准与Scaling Law | 精度相关Scaling Law、计算最优训练 |

- 适合:已经过一遍CS336/CS224N这类基础课,想知道"现在LLM研究圈到底在关注什么"的人
- 提示:这门课偏论文精读,不是从头教你写代码,建议有基础再看

## 实战部分(动手workshop,偏实践)

### Google & Kaggle · 5-Day AI Agents Intensive
- 官方页面:https://www.kaggle.com/learn-guide/5-day-agents
- 完全免费,现在是自学形式,累计超过150万学习者
- ⚠️ 需要注册一个免费Kaggle账号(不涉及信用卡,跟注册GitHub账号性质一样,不是Coursera那种藏起来的免费入口)
- 中文摘要:用Gemini + Google的Agent Development Kit动手搭一个真agent,已验证的真实主题包括Day1 Agent架构入门、Day2 工具调用与MCP互通、Day3 上下文工程与记忆(完整每日主题以官方页面为准)
- 适合:想直接上手搭一个能跑的agent,而不是先啃理论的人

### Anthropic · Building Agents with Model Context Protocol(Workshop)
- 视频:https://www.youtube.com/watch?v=kQmXtrmQ5Zg
- 完全免费,YouTube直接看,不用登录
- 主讲:Mahesh Murag(Anthropic)
- 中文摘要:一场完整的动手workshop,讲怎么用MCP给AI装上"手和脚",实操演示为主
- 适合:已经知道MCP是什么概念,想看具体怎么动手实现的人

### Anthropic · Code with Claude 开发者大会
- 主题演讲:https://www.youtube.com/watch?v=EvtPBaaykdo(其他城市站在YouTube搜"Code with Claude"就能找到)
- 配套workshop材料:https://github.com/anthropic/cwc-workshops
- 完全免费,演讲YouTube直接看不用登录;workshop仓库公开,可以直接照着做
- 中文摘要:Anthropic官方开发者大会内容,主题演讲讲行业趋势,workshop仓库是能照着做的实战材料
- 适合:想跟着Anthropic官方节奏,动手做agent/coding类项目的人

---
👉 顺序建议:CS230/CS224N打底 → CS336动手搭一个 → CS8803追前沿 → 实战部分随时可以插入练手。
