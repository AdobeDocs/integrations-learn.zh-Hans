---
title: 将 [!DNL Analytics] 和客户历程 [!DNL Analytics] 与Experience [!DNL Platform] 源连接器教程集成
description: 了解如何使用Experience [!DNL Platform] 源连接器将Adobe [!DNL Analytics] 与客户历程 [!DNL Analytics] 集成。
solution: Customer Journey Analytics, Target
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="集成" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
TQID: https://experienceleague.adobe.com/o3HCX8vz8ZKn2j1Hl3W4XWMOudx7MBZCMNRWxO-eKbw
product_v2: id: e43347a8-f2c5-4aa4-8623-6f13875d7e3aid: e98b7246-966c-4318-9e95-cad2f7a17dc7
feature_v2: id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5eid: f7c7de77-382f-4f48-8b36-61a170f06d3d
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 341
ht-degree: 18%

---

# 将Adobe [!DNL Analytics]和客户历程[!DNL Analytics]与Experience [!DNL Platform]源连接器集成

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">为要引入的数据创建架构</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">为要引入的数据创建数据集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架构</a>上配置正确的身份和身份命名空间，以确保摄取的数据可以拼合到统一配置文件。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为配置文件</a>启用架构和数据集。</li>
    <li>使用<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics]源连接器</a>将数据摄取到体验[!DNL Platform]</li>
    <li><i>（可选）</i>。 如果使用多个数据集，请将人员ID拼合在一起以<a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">生成组合数据集</a>。 如果使用单个[!DNL Analytics]数据集，或者如果您计划在客户历程[!DNL Analytics]中使用的所有数据集都存在通用标识符，请跳过此步骤。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">在客户历程[!DNL Analytics]中创建连接</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">创建数据视图</a>、<a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">配置组件设置</a>和<a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">格式化客户历程[!DNL Analytics]中的指标</a>。
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">在客户历程[!DNL Analytics]中创建项目。</a></li>
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics]源连接器的标准工作流步骤将创建用于从[!DNL Analytics]“原样”中摄取数据的架构和数据集。 因此，前两个步骤由系统处理。 映射工作流需要创建自定义属性；因此，请完全遵循一系列步骤。
