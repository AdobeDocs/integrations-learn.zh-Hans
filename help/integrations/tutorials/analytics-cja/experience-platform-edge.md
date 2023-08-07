---
title: 集成Adobe [!DNL Analytics] 和客户历程 [!DNL Analytics] 使用体验 [!DNL Platform] Edge教程
description: 了解如何集成Adobe [!DNL Analytics] 与客户历程 [!DNL Analytics] 使用AEP Web SDK、AEP Mobile SDK或Edge Network服务器API。
solution: Customer Journey [!DNL Analytics], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="集成" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 19%

---


# 集成Adobe [!DNL Analytics] 和客户历程 [!DNL Analytics] 使用体验 [!DNL Platform] Edge教程

<ol>
    <li>为要引入的数据<a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">创建架构</a>。</li>
    <li>为要引入的数据<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">创建数据集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架构上配置正确的身份和身份命名空间</a> 以确保摄取的数据可以拼合到统一的用户档案。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为配置文件启用架构和数据集</a>.</li>
    <li>将数据摄取到Experience [!DNL Platform] 使用以下方法之一：</li>
        <ul>
            <li>体验 [!DNL Platform] Web SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">教程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">清单</a></li>
                </ul>
            <li>体验 [!DNL Platform] 移动SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">教程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">清单</a></li>
                </ul></li>
            <li>边缘网络服务器 API:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">教程</a></li>
                </ul>
       </ul>
    <li><i>(可选)</i>. 如果使用多个数据集，请将人员ID拼合到 <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">生成组合数据集</a>. 如果使用单个 [!DNL Analytics] 数据集，或者您计划在客户历程中使用的所有数据集都存在一个通用标识符 [!DNL Analytics]，跳过此步骤。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">创建连接</a> 在客户历程中 [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">创建数据视图</a>， <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">配置组件设置</a>、和 <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">格式化量度</a> 在客户历程中 [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">在客户历程中创建项目 [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Adobe的标准工作流步骤 [!DNL Analytics] 源连接器创建用于从中摄取数据的架构和数据集 [!DNL Analytics] “原样”。 因此，前两个步骤由系统处理。 映射工作流需要创建自定义属性；因此，请完全遵循一系列步骤。
