### **DP-Rank-GRPO: Privacy-Preserving LLM Alignment**  
**NeurIPS 2027 (under review) | First student author (independent lead)**  

Proposed DP-Rank-GRPO to address the performance degradation of DP-PPO caused by injecting noise into high-dimensional policy gradients. The method generates a differentially private ranking of candidate responses at the scalar-reward level and maps the ranking to zero-mean advantage signals for policy optimization, avoiding DP-SGD and an additional value network.

#### Key Contributions:  
- Independently completed problem formulation, method design, privacy-theoretic analysis, algorithm implementation, experimental design, and paper writing.  
- Derived the pure ε-DP guarantee of the ranking mechanism based on the Exponential Mechanism and the Gumbel-Max trick.  
- Evaluated on Reddit TL;DR and IMDb with GPT-2, GPT-2 Medium and GPT-2 Large, systematically comparing non-private training, DP-PPO and the proposed method under different privacy budgets. The method maintains stable alignment under strict privacy constraints and outperforms gradient-level DP baselines on Reddit TL;DR.  

---

### **DP-Rank-GRPO：面向隐私保护的大语言模型对齐**  
**NeurIPS 2027（在投）| 学生一作（独立主导）**  

针对 DP-PPO 在高维策略梯度上注入噪声导致性能下降的问题，提出 DP-Rank-GRPO：在标量奖励端生成满足差分隐私的候选响应排序，并将排序映射为零均值优势信号进行策略优化，从而避免使用 DP-SGD 和额外价值网络。

#### 主要贡献:  
- 独立完成问题定义、方法设计、隐私理论分析、算法实现、实验设计与论文主体撰写。  
- 基于 Exponential Mechanism 与 Gumbel-Max trick 推导排序机制的 pure ε-DP 保证。  
- 在 Reddit TL;DR 与 IMDb 两类任务上，使用 GPT-2、GPT-2 Medium 和 GPT-2 Large，系统比较非私有训练、DP-PPO 与所提方法在不同隐私预算下的性能；结果显示，该方法在严格隐私约束下仍保持稳定对齐效果，并在 Reddit TL;DR 上优于梯度级差分隐私基线。  

---

### **HyperGumTree: Hypertree-based AST Representation for Long Code Diff Analysis**  
**ASE 2027 (under review) | Second student author**  

Proposed HyperGumTree, a code-block-aware AST representation based on Hypertree, to reduce the large node search space and matching overhead of AST-based code diff tools on long code files. Hyperedges aggregate semantically cohesive code blocks into unified structural units, preserving fine-grained syntactic information while transforming node-level matching into block-level matching. A three-stage mechanism—refined top-down, pruned bottom-up, and simple recovery—further improves the efficiency of long code diff analysis.

#### Key Contributions:  
- Responsible for method formalization, reproduction of comparison tools, and paper visualization.  
- Participated in defining the construction rules of Hypertree, BlockTypeSet and Hyperedge, and wrote the Preliminary and Methodology sections.  
- Reproduced 10 comparison tools, including the GumTree family, MTDiff, CLDiff, IJM, iASTMapper and HyperDiff, and conducted evaluations on Defects4J, GhJava, Refactoring Oracle and LongDiffEval. Results show 1.91× speedup, 47.7% runtime reduction and 11.1% smaller edit scripts on long code scenarios.  

---

### **HyperGumTree：面向长代码差异分析的 Hypertree AST 表征**  
**ASE 2027（在投）| 学生二作**  

针对 AST-based 代码差异分析工具在长代码文件中节点搜索空间大、匹配开销高的问题，提出基于 Hypertree 的代码块感知 AST 表征方法 HyperGumTree。该方法通过 Hyperedge 将语义内聚的代码块聚合为统一结构单元，在保留细粒度语法信息的同时，将节点匹配空间转化为块级表示，并结合 refined top-down、pruned bottom-up 与 simple recovery 三阶段机制提升长代码差异分析效率。

#### 主要贡献:  
- 负责方法形式化、对比工具复现与论文可视化。  
- 参与定义 Hypertree、BlockTypeSet 与 Hyperedge 构建规则，主笔 Preliminary 与 Methodology 相关内容。  
- 复现 GumTree 系列、MTDiff、CLDiff、IJM、iASTMapper、HyperDiff 等 10 个对比工具，并在 Defects4J、GhJava、Refactoring Oracle 与 LongDiffEval 上完成实验评估。结果显示，HyperGumTree 在长代码场景下实现 1.91× 加速、47.7% 运行时间降低，并减少 11.1% edit scripts size。  

---

### **Domestic Database Migration Evaluation Toolkit Adaptation**  
**2024.11 | Project Member**  

A key technical verification project responding to the "independent and controllable" strategy of China's energy industry. The project evaluated the replacement of the Oracle database currently used by Changqing Oilfield with domestic databases, and built a complete evaluation system covering high-concurrency OLTP performance (TPC-C), PB-scale data processing efficiency, long-term system stability, and security compliance. It quantitatively verified the technical feasibility and stability of replacing the original core business system with domestic databases under extreme workloads at the hundred-million-record scale.

#### Key Contributions:  
- Led the technical architecture research of multiple domestic database vendors and the selection and adaptation of an automated testing toolchain.  
- Studied and independently reproduced the BenchmarkSQL testing framework to address tool compatibility in heterogeneous environments.  
- Participated in defining a standardized test environment deployment plan, laying the foundation for subsequent vendor database testing standards.  

---

### **国产数据库迁移测评工具适配**  
**2024.11 | 项目成员**  

本项目是响应国家能源行业“自主可控”战略的关键技术验证工程，针对长庆油田当前使用的 Oracle 数据库，采用国产数据库替换的招投标项目深度评估。项目构建了涵盖高并发 OLTP 性能（TPC-C 模型）、PB 级数据处理效率、系统长稳性及安全合规的完整评价体系，通过模拟亿级数据规模下的极端业务负载，量化验证了国产数据库替代原有核心业务系统的技术可行性与稳定性。

#### 主要贡献:  
- 主导多品牌国产数据库的技术架构调研与自动化测试工具链的选型适配工作。  
- 针对异构环境下的工具兼容性难题，深入研究并二次测试复现了 BenchmarkSQL 测试框架。  
- 参与制定了标准化的测试环境部署方案，为项目后续各厂商数据库测试标准的制定奠定基础。
