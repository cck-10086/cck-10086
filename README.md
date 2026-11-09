# 崔程柯 · cck-10086

2027 届 · 绵阳城市学院 人工智能学院 · 计算机科学与技术
求职方向：**软件测试 / 技术支持 / 实施工程师**（成都 · 重庆 · 绵阳）

---

## 我做过什么

三个项目，一个主导、两个深度参与。下面每个项目都能点进去看代码、看提交记录、看测试文件。

### 🥇 [rental-platform](https://github.com/cck-10086/rental-platform) — 智能租房合同审查平台

毕业设计，独立完成。Java 21 + Spring Boot 3.4 + Vue 3 + DeepSeek + RAG。

**这个项目我最想讲的是"怎么知道它做对了"**：合同审查没有标准答案，所以我自建了 18 份合同的评测集、31 条埋入风险，跑了 5 轮迭代——精确率从 14.56% 提到 43.06%，F1 从 0.2532 提到 0.6019。

也是在这个过程里，我验证出自己加的规则引擎**是负贡献**（净 -4 条），最后选择保留架构、改策略，而不是硬说它有用。

- 11 张表、57 个 REST 接口
- 53 个自动化用例：45 个后端 JUnit（9 类）+ 8 个前端 Vitest
- 单次审查耗时 41.9s → 18.7s
- 28 次提交，有完整迭代历史

`Java` `Spring Boot` `Vue3` `MyBatis-Plus` `MySQL` `MinIO` `JWT` `RAG` `DeepSeek`

---

### 🥈 [city-travel](https://github.com/cck-10086/city-travel) — 城市轻旅行攻略与预订平台

课程综合实践，**4 人小组**。我负责前端全量页面、数据统计模块、AI 行程规划模块。

Spring Boot 2.7 + Spring Security + MyBatis-Plus + Redis + DeepSeek，原生 HTML/CSS/JS 前端。

几处设计我可以说清为什么：订单金额**服务端重算**不信任前端；AI 返回结构化 JSON 且有本地规则兜底；Redis 做配额、缓存、成本统计三件事。

交付时仓库里只有 1 个冒烟测试，**我补到 17 项**（我负责的模块 5 项，其余替组员模块补的）。

`Java` `Spring Boot` `Spring Security` `Redis` `MyBatis-Plus` `ECharts` `DeepSeek`

---

### 🥉 [YOLOv8-Detector](https://github.com/cck-10086/YOLOv8-Detector) — 光伏电池片 EL 缺陷检测

课程论文项目，个人完成。基于 YOLOv8 做坐标注意力（C2f_CA）的位置消融实验。

mAP50 从 88.04% 提到 90.17%，但**召回率从 84.17% 掉到 82.04%**——这个退化我没藏，归因是小目标样本不足叠加增强过强。

四组位置消融里，颈部插入那组只有 67.54%，掉了 20 个点。这个反例比正例更有信息量：注意力插在哪，比注意力本身更重要。

**这是算法应用，不是算法研究**——注意力模块本身是已有工作，我做的是验证和归因。

`PyTorch` `YOLOv8` `ONNX` `OpenCV` `PVEL-AD`

---

## 关于我的工作方式

我大量使用 AI 辅助写代码。**AI 负责生成和提速，我负责定义什么叫对、以及验收。**

具体到我做的事：架构方向、评测集怎么设计、指标怎么定义、每轮改什么、哪些结论可以对外说。规则引擎是负贡献那个结论，就是我自己逼着逐条归因才敢下的。

所以我不会说"每一行都是我敲的"，但每一行为什么这么写，我能解释。

---

## 技术栈

| 类别 | 内容 |
|---|---|
| 语言 | Java、Python、SQL、JavaScript |
| 后端 | Spring Boot、Spring Security、MyBatis-Plus、JWT |
| 数据 | MySQL（建表/索引/多表查询）、Redis（缓存/配额） |
| 测试 | JUnit 5、Mockito、Vitest、接口测试、缺陷复现与归因 |
| AI 应用 | DeepSeek API、LangChain4j、RAG、提示词迭代与评测 |
| 视觉 | PyTorch、YOLOv8、ONNX、OpenCV |
| 工程 | Git、Linux 常用排查、MinIO、Docker 基础 |

---

## 联系

- 📧 3447376162@qq.com
- 📍 四川资阳 · 在绵阳读书 · 可到岗时间 2026-11-09
