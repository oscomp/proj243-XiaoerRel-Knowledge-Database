# proj243-XiaoerRel-Knowledge-Database
### 项目名称
社区问答助手"龙蜥小二"语料库收集

### 支持单位
[龙蜥社区 (OpenAnolis)](https://openanolis.cn/)

### 项目描述

"龙蜥OpenAnolis社区交流群"（钉钉群号：29935009584），通过龙蜥小二提供社区和操作系统相关智能检索和知识文档的服务。当前人工智能技术的快速发展，如通义千问和 ChatGPT，对交互服务的变革创造了新的可能，也提出了新的要求。为了更好的服务社区用户，龙蜥小二会进行进一步的智能优化。

### 所属赛道

2023 全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生或研究生（2023年春季学期或之后毕业的大一~大四的本科生或研究生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2023全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

问书

* github https://github.com/WeissonHan/

* email wenshu.hx@alibaba-inc.com



### 难度

中等



### 特征

- 整理收集龙蜥社区官网文档和 Linux 系统知识问答语料，此类语料面向龙蜥社区以及 Linux 生态操作系统的用户。
- 对数据按照验收要求进行关系抽取梳理，当用户通过龙蜥小二提问时，从用户提问中提取关键信息（Subject 与 Predict），并给出相应解答（Object）；
- 我们需要这些语料去训练模型（通义千问或者 ChatGPT），单次训练需要 1000+ 条。训练完成后，可以帮助龙蜥小二服务用户问题。

### License

[MulanPSL-2.0](https://opensource.org/license/mulanpsl-2-0/)



## 预期目标
1. 原始语料数据集和关系梳理后的数据集；

   具体要求：
   * 关系梳理后的数据集以无表头的 csv 的格式给出，采用 utf-8 编码，每一行的数据以 Subject, SubjectEmbedding, Predict, PredictMatrix, Object, ObjectEmbedding 的格式储存，对 SubjectEmbedding、PredictMatrix、ObjectEmbedding 的维数与格式不做要求，列之间以逗号分隔即可；
   * 有效数据（SPO 三元组）不少于 1000。
2. 关系梳理（数据清洗、关系抽取、数据查询）等相关逻辑的代码库；

   具体要求：
   * 关系抽取与数据查询的逻辑会直接用于最终项目的评测，请注意提交代码的完整性。
3. 关系梳理逻辑项目书；

   具体要求：
   * 项目书应当在 4000 字以上，表达清晰、逻辑明确，建议以 `摘要、引言、数据清洗、关系抽取设计、实验结果、总结` 的结构划分章节。

## 备注

### 评价标准：

1. 有效三元组(SPO)数量 (40%)；
2. 题库中随机抽取 200 条提问对查询的关联程度 (30%)；
3. 项目书的行文逻辑以及可实践性 (20%);
4. 奖励分，用于鼓励在保证项目完成质量的基础上，打破题目框架限制并做出额外亮眼表现的团队 (10%)。
