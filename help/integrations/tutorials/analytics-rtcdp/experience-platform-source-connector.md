---
title: 集成 [!DNL Analytics] 和实时客户数据 [!DNL Platform] 具有体验 [!DNL Platform] 源连接器教程
description: 了解如何集成Adobe [!DNL Analytics] 使用实时客户数据 [!DNL Platform] 使用体验 [!DNL Platform] 源连接器。
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="集成" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 19%

---


# 集成Adobe [!DNL Analytics] 和实时客户数据 [!DNL Platform] 具有体验 [!DNL Platform] 源连接器

<ol>
    <li>为要引入的数据<a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">创建架构</a>。</li>
    <li>为要引入的数据<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">创建数据集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架构上配置正确的身份和身份命名空间</a> 以确保摄取的数据可以拼合到统一的用户档案。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为配置文件启用架构和数据集</a>.</li>
    <li>摄取 [!DNL Analytics] 使用将数据导入Experience Platform <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] 源连接器</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">在Experience中创建区段 [!DNL Platform].</a> 系统自动确定评估该区段是批处理（数据连接器）还是流式传输（边缘网络）。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">配置目标以将配置文件属性和受众成员身份共享到所需目标。</a></li>   
</ol>

>[!NOTE]
>
>Adobe的标准工作流步骤 [!DNL Analytics] 源连接器创建用于从中摄取数据的架构和数据集 [!DNL Analytics] “原样”。 因此，前两个步骤由系统处理。 映射工作流需要创建自定义属性；因此，请完全遵循一系列步骤。
