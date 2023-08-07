---
title: 集成 [!DNL Analytics] 替换为 [!DNL Commerce] 教程
description: 了解如何集成 [!DNL Analytics] 替换为 [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="集成" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 5%

---


# 集成 [!DNL Analytics] 替换为 [!DNL Commerce]

## 初始载入

这些说明适用于Adobe [!DNL Commerce] 云托管项目。 自托管在某种程度上可能有所不同，但整个过程应该相似。

1. 在本地环境中查看代码
1. 使用编辑器和安装模块
1. 请按照此处的各个说明进行操作，并在完成后返回以完成剩余步骤
   [安装和配置体验 [!DNL Platform] 连接器](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. 提交composer.json，如果在云中，则提交composer.lock文件
1. 验证模块是否在暂存和/或生产环境中。为此，您可以登录Adobe的“管理员”部分 [!DNL Commerce] 并在System > Services下查找这些新部分
   ![体验 [!DNL Platform] 连接器扩展](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. 使用Adobe中的凭据配置模块 [!DNL Commerce] 后台。
   * 首先 [!DNL Commerce] 服务连接器配置，如下所示。
     ![[!DNL Commerce] 服务连接器设置](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * 然后是体验 [!DNL Platform] 连接器设置，如下所示。
     ![体验 [!DNL Platform] 连接器](./assets/analytics-commerce/experience-platform-connector.png)

有关载入流程的每个阶段和步骤的更多详细信息，请按照 [体验 [!DNL Platform] 连接器概述](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. 体验 [!DNL Platform] 连接器教程将深入介绍每个部分，并解答您遇到的任何问题。 使用本教程了解其余快速设置步骤。

## Experience Edge和Adobe的配置 [!DNL Analytics]

1. 验证您的组织是否拥有（并且您拥有）Adobe的访问权限 [!DNL Analytics]. 这可以通过转到 [Adobe Experience Cloud主页](https://experience.adobe.com/) ，然后单击顶部导航中的应用程序切换器（九个点）。

1. 在Adobe中创建新报表包 [!DNL Analytics]，或标识您将推送的报表包的ID [!DNL Commerce] 将数据传入。 有关更多信息，请观看上的教程 [创建新报表包](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html). 您在下面的数据流步骤中需要此报表包ID。

1. 导航至 [Adobe Experience [!DNL Platform] 界面](https://platform.adobe.com) 如果您有权访问Experience [!DNL Platform]. 如果您无权访问该界面，则可以在Adobe Experience中执行下面列出的所有必要步骤 [!DNL Platform] [数据收集界面](https://experience.adobe.com/#/data-collection).

1. 使用以下方式创建或更新您的XDM架构 [!DNL Commerce]特定字段组。 有关如何创建架构的更多信息，请参阅 [&quot;创建模式&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html) 教程。
   * 您将需要从下面数据流步骤中的选项中选择此架构。 要创建架构，请查看左列中的 **数据管理** 并查找 **架构**. 现在，在界面的右上方，单击 **创建架构**. 选择XDM ExperienceEvent。
   * 创建新架构后，您将添加 [!DNL Commerce] 字段组。 在UI的左侧，找到字段组，然后单击 **添加**
      * 在搜索中，您可以通过输入以下内容进行过滤 `ExperienceEvent [!DNL Commerce]`
      * 选择 **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** 勾选方框
      * 然后单击 **添加字段组** 保存并继续

1. （可选，并且仅在您处于体验中时） [!DNL Platform] 界面) — 创建新数据集
   * 此步骤允许您将 [!DNL Commerce] 将数据导入Experience [!DNL Platform] (独立于将数据导入Adobe [!DNL Analytics])。 如果您有权访问Experience，请执行此步骤 [!DNL Platform]，并计划使用 [!DNL Commerce] 体验中的数据 [!DNL Platform] — 支持的应用程序，如实时客户数据 [!DNL Platform]，客户历程 [!DNL Analytics]或Journey Optimizer。
   * 您将需要从下面数据流步骤中的选项中选择此数据集。
   * 在左列下 **数据管理** 标题在左侧导航中，选择 **数据集**.
   * 单击 **创建数据集** 在右上角。 选择 **从架构创建数据集** 选项。
   * 搜索并使用您在上一步中创建的架构

1. 创建数据流以发送 [!DNL Commerce] 要Adobe的数据 [!DNL Analytics]
   * 在 **数据收集** 标题中，选择 **数据流**.
   * 单击 **新建数据流** 界面右上角的。
   * 提供名称、说明和可选说明。
   * 查找并选择您在上一步中创建/标识的架构。
   * 添加任何所需的高级选项。 欲知关于高级选项的更多信息，请访问 [文档](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=zh-Hans).
   * 单击 **保存** 以继续。
   * 单击 **添加服务** 并选择 **Adobe[!DNL Analytics]** （在下拉字段中）。
   * 单击 **添加报表包** 并输入您在上一步中创建/识别的报表包ID。 如果希望数据流入多个报表包，您可以添加多个报表包。
   * 或者，如果您在上一步中创建了一个数据集，请单击 **添加服务** 再次选择 **Adobe Experience[!DNL Platform]** 从下拉字段中。 在事件数据集字段中，选择之前创建的数据集。
   * 保存数据流。

1. 最后，查看 [!DNL Commerce] 因此，您需要在Adobe中导航到Analysis Workspace [!DNL Analytics]，创建一个项目，选择您的报表包，然后添加自由格式表和其他可视化图表以报告和分析 [!DNL Commerce] 数据。 下图显示了您可以在Analysis Workspace中创建的表的一个示例。

   ![[!DNL Analytics] 某些商业数据的屏幕截图](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   以下是帮助您在Analysis Workspace中工作的一些其他资源：

   * [Analysis Workspace 概述](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [从头开始构建 Workspace 项目](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [使用 Analysis Workspace 中的表、可视化和面板](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [可视化图表用例](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   此外，还提供免费的Experience League课程。 请参阅 [!DNL Analytics] 可用课程 [此处](https://experienceleague.adobe.com/?lang=en&amp;Solution=[!DNL Analytics]#courses)。
