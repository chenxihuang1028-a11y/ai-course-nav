# 02 · 工程师转 Agent / AI Infra

适合有编程基础,想从传统SDE转向AI Infra、大模型训练、Agent开发方向的人。建议按下面顺序看。

## 入门顺位

### Stanford CS336 · Language Modeling from Scratch
- 2025版playlist:https://www.youtube.com/playlist?list=PLoROMvodv4rOY23Y0BoGoBGgQ1zmU_MT_
- 2026版playlist:https://www.youtube.com/playlist?list=PLoROMvodv4rMqXOcazWaTUHhq-yembLCV
- 中文摘要:从零手写一个语言模型,覆盖数据处理、Tokenization、Transformer架构、训练、并行、推理、评测全流程。目前公认转LLM工程方向最扎实的一门课,业内讨论"转型AI Infra看这个就够"通常指的就是它。
- 已知讲座(按标题,非精确时间戳):Lecture 1 Overview & Tokenization / Lecture 3 Architectures / Lecture 10 Inference,完整列表见playlist

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

---
👉 顺序建议:CS230/CS224N打底 → CS336动手搭一个 → CS8803追前沿。
