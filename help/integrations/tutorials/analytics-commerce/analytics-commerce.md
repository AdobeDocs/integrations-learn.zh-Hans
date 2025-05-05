---
title: 将 [!DNL Analytics] 与 [!DNL Commerce] 教程集成
description: 了解如何将 [!DNL Analytics] 与 [!DNL Commerce]集成。
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
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# 将[!DNL Analytics]与[!DNL Commerce]集成

## 初始载入

这些说明适用于Adobe[!DNL Commerce]云托管项目。 自托管在某种程度上可能有所不同，但整个过程应该相似。

1. 在本地环境中查看代码
1. 使用编辑器和安装模块
1. 请按照此处的各个说明进行操作，并在完成后返回以完成剩余步骤
   [安装和配置Experience [!DNL Platform] 连接器](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. 提交composer.json，如果在云中，则提交composer.lock文件
1. 验证模块是否在暂存和/或生产环境中
为此，您可以登录Adobe[!DNL Commerce]的“管理员”部分，然后在“系统”>“服务”下查找这些新部分
   ![体验[!DNL Platform]连接器扩展](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. 使用Adobe[!DNL Commerce]后台中的凭据配置该模块。
   * 首先是[!DNL Commerce]服务连接器配置，如下所示。

     ![[!DNL Commerce]服务连接器安装程序](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * 然后是Experience [!DNL Platform]连接器设置，如下所示。

     ![体验[!DNL Platform]连接器](./assets/analytics-commerce/experience-platform-connector.png)

有关载入流程的每个阶段和步骤的更多详细信息，请按照[Experience [!DNL Platform] 连接器概述](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}中的说明操作。 Experience [!DNL Platform]连接器教程深入涵盖了每个部分，并回答您可能遇到的任何问题。 使用本教程了解其余快速设置步骤。

## Experience Edge和Adobe[!DNL Analytics]的配置

1. 验证您的组织是否具有（并且您具有）访问Adobe[!DNL Analytics]的权限。 可以通过转到[Adobe Experience Cloud主页](https://experience.adobe.com/)并单击顶部导航中的应用程序切换器（9个点）来确认这一点。

1. 在Adobe[!DNL Analytics]中创建新报表包，或确定您将[!DNL Commerce]数据推入的报表包的ID。 有关详细信息，请观看有关[创建新报表包](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html)的教程。 您在下面的数据流步骤中需要此报表包ID。

1. 如果您有权访问Experience [!DNL Platform]，请导航到[AdobeExperience [!DNL Platform] 界面](https://platform.adobe.com)。 如果您无权访问该界面，则可以在AdobeExperience [!DNL Platform] [数据收集界面](https://experience.adobe.com/#/data-collection)中执行下面列出的所有必要步骤。

1. 使用特定于[!DNL Commerce]的字段组创建或更新您的XDM架构。 有关如何创建架构的更多信息，请参阅[“创建架构”](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html)教程。
   * 您将需要从下面数据流步骤中的选项中选择此架构。 要创建架构，请在&#x200B;**数据管理**&#x200B;下的左列中查找&#x200B;**架构**。 现在，在界面的右上角，单击&#x200B;**创建架构**。 选择XDM ExperienceEvent。
   * 创建新架构后，您将添加[!DNL Commerce]字段组。 在UI的左侧，查找字段组，然后单击&#x200B;**添加**
      * 在搜索中，您可以通过输入`ExperienceEvent Commerce`进行筛选
      * 通过勾选方框选择&#x200B;**Adobe[!DNL Analytics] ExperienceEvent[!DNL Commerce]**
      * 然后单击右上方的&#x200B;**添加字段组**&#x200B;以保存并继续

1. （可选，并且仅当处于Experience [!DNL Platform]界面中时） — 创建新数据集
   * 此步骤允许您将[!DNL Commerce]数据引入Experience [!DNL Platform] (与将数据引入Adobe[!DNL Analytics]分开)。 如果您有权访问Experience [!DNL Platform]，并计划在支持Experience [!DNL Platform]的应用程序中使用[!DNL Commerce]数据，如实时客户数据[!DNL Platform]、客户历程[!DNL Analytics]或Journey Optimizer，请执行此步骤。
   * 您将需要从下面数据流步骤中的选项中选择此数据集。
   * 在左侧导航的左列&#x200B;**数据管理**&#x200B;标题下，选择&#x200B;**数据集**。
   * 单击右上方的&#x200B;**创建数据集**。 选择&#x200B;**从架构创建数据集**&#x200B;选项。
   * 搜索并使用您在上一步中创建的架构

1. 创建数据流以将[!DNL Commerce]数据发送到Adobe[!DNL Analytics]
   * 在左列中的&#x200B;**数据收集**&#x200B;标题下，选择&#x200B;**数据流**。
   * 单击界面右上角的&#x200B;**新建数据流**。
   * 提供名称、说明和可选说明。
   * 查找并选择您在上一步中创建/标识的架构。
   * 添加任何所需的高级选项。 有关高级选项的详细信息，请访问[文档](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=zh-Hans)。
   * 单击&#x200B;**保存**&#x200B;以继续。
   * 单击&#x200B;**添加服务**，然后在下拉字段中选择&#x200B;**Adobe[!DNL Analytics]**。
   * 单击&#x200B;**添加报表包**，然后输入您在上一步中创建/识别的报表包ID。 如果希望数据流入多个报表包，您可以添加多个报表包。
   * 或者，如果您在上一步中创建了一个数据集，请再次单击&#x200B;**添加服务**，然后从下拉字段中选择&#x200B;**Adobe体验[!DNL Platform]**。 在事件数据集字段中，选择之前创建的数据集。
   * 保存数据流。

1. 最后，要查看[!DNL Commerce]数据，您需要导航到Adobe[!DNL Analytics]中的Analysis Workspace、创建项目、选择报表包以及添加自由格式表和其他可视化图表来报告和分析[!DNL Commerce]数据。 下图显示了您可以在Analysis Workspace中创建的表的一个示例。

   ![[!DNL Analytics]某些商业数据的屏幕截图](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   以下是帮助您在Analysis Workspace中工作的一些其他资源：

   * [Analysis Workspace 概述](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [从头开始构建Workspace项目](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [在Analysis Workspace中使用表、可视化和面板](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [可视化使用案例](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   此外，还提供免费的Experience League课程。 查看[此处](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses)提供的[!DNL Analytics]课程。
