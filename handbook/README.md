<div class="hero">
  <h1>AI 合规工程</h1>
  <div class="sub">从监管到证据：可信与伦理 AI 系统的方法论<br/>把法律与政策语言的监管要求，转译为可落地的技术控制，并用可审计的证据证明控制有效。</div>
  <div class="badges"><span>作者 ZhiXuan ZHU</span><span>AI 合规 · 大模型安全 · 风险治理</span><span>ISBN 979-8-16714-909-0</span></div>
</div>

## 这个站点讲什么

监管要求以法律和政策语言表达，而 AI 系统由代码、架构和运营流程构建。治理框架（如 NIST AI RMF、ISO/IEC 42001、欧盟《人工智能法案》）说明了*应该做什么*，却很少说明*如何在技术上实施*；安全工程实践解决了*如何控制特定风险*，却缺乏与监管要求和证据标准的系统连接。

本站把**监管（Regulation）— 控制（Controls）— 证据（Evidence）**视为同一个工程问题，沉淀一套可复用的转译方法、映射表、自查清单与证据模板。它是著作《AI 合规工程》的公开方法论站点，用于交流与求职 / 研究成果展示；完整论证、案例与操作细节以正式出版物为准。

## 四个方法构件

<div class="cards">
  <div class="card"><h4>CTF 合规转译框架</h4><p>Compliance Translation Framework：把抽象监管要求，经四个抽象层级系统性转化为具体技术控制与验证证据的组织框架。</p></div>
  <div class="card"><h4>RCE 风险—控制—证据闭环</h4><p>Risk-Control-Evidence：让风险识别、控制实施与证据生成形成闭环迭代，而非彼此脱节的活动；在控制设计阶段就规定要产出的证据。</p></div>
  <div class="card"><h4>PTB 提示信任边界</h4><p>Prompt Trust Boundary：在生成式 AI 中建模系统指令、开发者配置与不可信外部内容之间的权限边界，核心原则是低信任信息不得修改高信任规则。</p></div>
  <div class="card"><h4>FTH 事实信任层级</h4><p>Fact Trust Hierarchy：生成声明的置信度不应超过其所依据信息来源的信任等级，为检索增强与工具输出提供来源约束。</p></div>
</div>

> 定位说明：CTF 与 RCE 属于组织框架，用于整合既有成熟实践；PTB 与 FTH 是设计主张（概念模型），尚未作为预测模型经过正式实证验证，不应被当作定量定律使用。

## 站内导航

- [方法论框架](docs/framework.md)：四个构件的定义、相互关系与适用边界。
- [法规—证据映射](docs/regulation-map.md)：欧盟《人工智能法案》核心义务 → 所需证据工件 → 对应工程方法。
- [OWASP LLM Top 10 交叉映射](docs/owasp-map.md)：从攻击类别快速跳到法案义务与对策章节。
- [证据工件模板](docs/evidence-templates.md)：AI 系统清单、风险登记册、附件 IV 技术文档清单等可直接套用的表格。
- [合规自查清单](docs/checklist.md)：面向输入端、运行中、出错后的“三大缺口”体检与治理清单。
- [验证与红队方法](docs/verification.md)：基准测试、红队测试、可解释性与持续监控的验证思路。
- [章节导览](docs/chapters.md)：全书 16 章与附录的结构地图。
- [术语表](docs/glossary.md)：CTF / RCE / PTB / FTH、RAG、提示注入、FRIA、GPAI 等术语速查。
- [关于作者与免责声明](docs/about.md)

<div class="book-cta">
  <strong>正式出版物：《AI 合规工程：从监管到证据——可信与伦理 AI 系统方法论》</strong><br/>
  完整章节、端到端案例研究、附录 A–D 方法论与法规证据索引，见正式平装 / 电子书。
  <br/><a class="btn" href="https://www.amazon.com/dp/B0HQDC7HJ2" target="_blank" rel="noopener">在 Amazon 查看本书</a>
</div>

## 适合谁

- 需要把合规要求写进架构与代码的 **AI / 安全工程师**；
- 负责 AI 风险、内控、审计与尽职调查的**合规与风控人员**；
- 评估高风险 AI 落地的**技术管理者与产品负责人**；
- 关注 AI 治理、算法公平与生成式 AI 安全的**研究者与学生**。

---

*本站内容为方法论科普与工程参考，不构成法律意见；具体合规判定请结合司法管辖区、行业与用例咨询合格法律顾问。*
