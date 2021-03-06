[PhyLab1.0需求规格说明文档](https://github.com/buaase/Phylab-Web/blob/master/docs/Require-Specification.md#3%E7%95%8C%E9%9D%A2%E5%8E%9F%E5%9E%8B)

# 1. 概述

## 1.1 项目概述

**软剑攻城队**小组于2015学年开发了**PhyLab**物理实验网站，一经发布好评如潮。网站的核心功能是**提供预习报告**和**自动数据处理**，而后加入了论坛模块，提供了一定的社交功能。前续版本总体满足了目标用户的需求，但是在实际使用过程中存在数据计算错误、模板无法生成、按钮失效等Bug，流失了大量的二次用户。目前开发项目为PhyLab的**2.0版本**，α阶段的开发中心主要是在完善实验内容、实现未完成功能、提高前端用户体验，并加入诸如实时数据处理结果预览、输入数据显性纠正、实验处理工具等改进型功能。在β阶段再考虑加入革命性的核武器级功能。

## 1.2 开发信息

* 项目名称：PhyLab2.0
* 目标用户：北京航空航天大学本科二年级理工科学生
* 开发团队：**Default团队**
* 发布位置：Internet
* 发布一周用户量（15级）：250名

# 2. NABCD模型

## 2.1 N（Need 需求）

PhyLab1.0需求规格说明文档以及网站的实践已经证明了北航大二学生有着较强的需求，当前用户的累计注册量已经达到了900，占所有必修学生数量的1/5，反馈情况较好。但是目前只是解决了需求层次的**温饱**问题，在随访中很多学生在使用过一两次后就不再使用了，这是由于报告生成存在不少问题，比如花费大量时间输入数据后无法生成模板、无法对错误数据录入进行详情提示、实验报告模板跟不上实际实验变化等，让用户对PhyLab失去了信心。所以目前用户最大的需求就是**稳定的全实验模板生成功能**，这是极大的刚性需求，也是PhyLab的立命之本。当然大约30%用户比较关注拓展功能，比如**通用实验数据处理工具**、**简便的社交功能**、**实验数据纠正**等，这是属于辅助性需求，在稳定核心功能后进一步改进用户体验。由于每学年都有大量学生需要必修物理实验，都形成稳定的用户群体，大概为3000名，需求巨大稳定。本学期的第1周至15周，大概有**3500名**在校学生需要必修物理实验，完全处于PhyLab的开发周期中，可以在不断的反馈中进行迭代改进。

## 2.2 A（Approach 做法）

目前PhyLab已经实现了基本的核心功能，添加了一定的社交功能。但是实际上核心功能不完善，模板残缺，用户黏度较低。我们会投入大量资源，核验当前“实验报告模板”，确保每一份预习报告都可以完整翔实，同学在借鉴后通过率达到99%。对于“实验数据处理报告”，目前的问题还很大，比如数据录入方式简陋、部分实验未实现、实验处理脚本残缺等，这是PhyLab的核心竞争功能，不应该存在较多的问题，所以**全面支持所有实验（且正确）**是α阶段的核心任务。鉴于PhyLab网站框架已经搭建完毕，时间较为充沛，可以把精力放到网站内容上。我们将精选标准优质的数据处理原始报告，仔细核对所有计算步骤、表格、公式，将其**准确数据化**于PhyLab中。最后添加相应的辅助功能，**优化用户的前端体验**，提高用户粘性。团队中的两名后端主力编码能力极强，参与编写过多个正式网站工程，经验丰富，可以较快实现目标功能。且大家都经历过物理实验，均可以参与到内容整理和制作上来。

## 2.3 B（Benefit 好处）

由于以往残缺的用户体验，未明确标示模板是否可用，计算脚本是否可用，浪费了用户的大量时间。造成用户对网站的信心较低，甚至开始怀疑模板与数据处理是否正确。2.0版本通过稳定并完善核心的**实验报告生成**功能，使得用户可以**真正**一站式解决所有的实验预习报告和数据处理报告的相关问题。摆脱繁琐的手工处理，通过数字化的辅助将每份实验报告撰写时间控制在2~4小时，去除不必要的**资料收集**、**肉眼辨识**、**繁琐计算**等工作。通过调查统计，平均每个实验每人次可节约**1~2小时**，且基本可以**一次通过**拿到较高的分数。总结起来就是八个字**省时、省心、高分通过**。并且为照顾学生对交流的需求，加入了社交功能，可以进行**答疑、交流、资源分享**，具有较强的拓展性，社交系统中累积了大量有价值的第三方信息与资源，满足了信息共享的需求。

## 2.4 C（Competitor 竞争）

目前每年的市场的校内市场规模在3500人左右，基本固定，不太可能增长和缩减。可以通过增加网站的通用性，推广到其它学校，进入到全国的市场行列中，但是暂时没有这个考虑。通过宣传和推广预计可以使得40%（1500）的同学得知网站的存在，对一个第三方非盈利性校内网站来说有着广阔的市场。市场上暂时没有任何和PhyLab功能类似的网站，只有相关的信息资源共享平台，其特征如下：

| 平台 | 优点 | 缺点 |
| --- | --- | --- |
| 基础物理实验选课网 | 1. 注册用户极多，流量大。 2. 提供信息资源权威准确。 | 1. 交互界面简陋。 2. 讲义较少，且PPT信息冗余。 3. 无社交功能。 |
| QQ群 | 1. 交流性极强。 2. 任何人都可以进行资源分享。 3. 相关信息更新及时。 | 1. 过往信息难回溯查看。 2. 信息杂乱，不成体系。 3. 资源质量和可信度较差。 |
| 百度文库 | 1. 极易使用和查找。 2. 访问方便简单。 | 1. 资源杂乱，质量参差不齐。 2. 无社交功能。 |

所以目前几乎没有市场竞争，我们只需要做好**实验报告生成**和**权威资源共享**功能，基本可以全占整个市场。再通过加强论坛社交功能，基本可以涵盖所有竞品的功能，形成垄断地位。唯一缺点是我们是非盈利性组织，没有固定的维护团队，成员的工程实力较差。

## 2.5 D（Delivery 交付）

Web的优势就是不需要下载和商店入驻，只要接入了Internet就可以访问。所以只要进行相应的宣传，并提高用户黏度即可。为了进行推广我们将尽力联合北航**公众微信号**（北航推荐、北航新鲜事、北航社联、北航学生会等）进行线上传播，由于“撰写物理报告”刚需的特殊性，且在2014级已经有一定的知名度，借助**朋友圈**或QQ空间可以较快进行传播和推广。其次，如果项目达到了我们的目标水平，**全面稳定覆盖物理实验**，我想只要用过的同学肯定会推荐给身边的人，出现病毒式传播的现象。

# 当前功能分析

# 用户反馈

# 功能改进方案