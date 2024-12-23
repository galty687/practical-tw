# 技术文档质量

技术文档的质量是一个系统工程，整体是由“人+流程+工具”来保证的。

## 人

从事技术写作的人员应接受过相应的教育，这里可以是某个技术写作的本科专业，或者通过了系统化的培训来获得，例如 [STC Certification](https://www.stc.org/certification/)、[Tekom Certification](https://www.technical-communication.org/technical-writing/tekom-certification) 和中国标准化协会技术传播服务委员会均有相应的课程。


## 流程

流程是做一件事情的基本步骤，例如我们可以参加 [IEC 82079](https://www.iso.org/standard/71620.html) 的流程规定。



## 工具

使用各种工具降低人的负担，提高流程的可靠性。




## 技术文档质量的层次
- 准确性
- 可用性
- 用户体验/信息体验

好的文档应能确保内容的准确性，在此基础之上要考虑可用性，最后考虑整体的信息体验。

### 准确性
在确保内容准确性上，目前通常从如下几个方面做约束。

#### 内容结构标准

使用DITA将内容的结构和模块进行标准化。使用oXygen XML 基于 DTD 或 Schema 来 Validate DITA 内容，确保DITA的正确性。

#### 受限语言

使用受限语言降低内容的难度，确保内容的一致性。例如 [ASD-STE](https://asd-ste100.org/)语言。 

#### 语言检测工具
文本的准确性通常可以从以下三个方面来检测。

  - 拼写
  - 句法
  - 风格



| 工具                                       | 性质      | 功能                       |
| ------------------------------------------ | --------- | -------------------------- |
| [Langauge Tool](https://languagetool.org/) | 开源+商业 | 可自定义规则检测文档风格   |
| [ProseLint](http://proselint.com/)         | 开源      | 可通过命令行检测文本质量   |
| [Acrolinx](https://www.acrolinx.com/)      | 商业      | 完整的文档质量检查解决方案 |



| 指标           | 含义 | 计算方式 |
| -------------- | ---- | -------- |
| Readability    | 评价文档阅读的难易程度 | [文档](https://readable.com/readability/flesch-reading-ease-flesch-kincaid-grade-level/) |
| Coh-Metrix | 评价文档的衔接程度 | [文档](http://cohmetrix.memphis.edu/cohmetrixhome/documentation_indices.html) |



## 可用性

内容准确的资料用户未必觉得好用，重要的资料还需要做可用性测试，确保内容的可用性。

关注的指标：

- 完成率。使用资料完成任务的概率。
- 效率。使用资料完成任务的时间。
- 满意度。大众使用资料后的满意程度。



## 用户体验/信息体验设计

在确保了内容准确性和可用性的基础之上，则可以探索内容的信息体验，让用户阅读时有赏心悦目，喜闻乐见的同时，增强用户粘性 。



[comment]: # "This actually is the most platform independent comment"



[](Comment text goes here)

