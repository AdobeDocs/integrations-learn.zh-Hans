---
title: 将 [!DNL Analytics] 和实时客户数据 [!DNL Platform] 与Experience [!DNL Platform] 源连接器教程集成
description: 了解如何使用Adobe [!DNL Platform] 源连接器将Experience [!DNL Analytics] 与实时客户数据 [!DNL Platform] 集成。
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="集成" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
TQID: https://experienceleague.adobe.com/Uct30-UadP-2Ocwslbk-dMAV0Y2unZlA339hThnofpA
product_v2: id: e55547f1-a1ff-40c6-8978-026e40ab7fa4id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
subfeature_v2: id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 11%

---

# 将Adobe [!DNL Analytics]和实时客户数据[!DNL Platform]与Experience [!DNL Platform]源连接器集成

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">为要引入的数据创建架构</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">为要引入的数据创建数据集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架构</a>上配置正确的身份和身份命名空间，以确保摄取的数据可以拼合到统一配置文件。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为配置文件</a>启用架构和数据集。</li>
    <li>使用<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics]源连接器</a>将[!DNL Analytics]数据摄取到Experience Platform。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">在体验[!DNL Platform]中创建区段。</a> 系统会自动确定评估区段是批处理（数据连接器）还是流式传输（Edge网络）。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">配置目标以将配置文件属性和受众成员身份共享到所需目标。</a></li>   
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics]源连接器的标准工作流步骤将创建用于从[!DNL Analytics]“原样”中摄取数据的架构和数据集。 因此，前两个步骤由系统处理。 映射工作流需要创建自定义属性；因此，请完全遵循一系列步骤。
