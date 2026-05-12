---
title: 将 [!DNL Analytics] 和实时客户数据 [!DNL Platform] 与Experience [!DNL Platform] Edge教程集成
description: 了解如何使用Adobe Web SDK、AEP Mobile SDK或Edge Network服务器API将AEP [!DNL Analytics] 与实时客户数据 [!DNL Platform] 集成。
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="集成" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
TQID: https://experienceleague.adobe.com/K1CpRtUekl5jQNDMGswJpexC9fv9uVmgraLlNFXUIr8
product_v2: id: e55547f1-a1ff-40c6-8978-026e40ab7fa4id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
subfeature_v2: id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 8%

---

# 将Adobe [!DNL Analytics]和实时客户数据[!DNL Platform]与Experience [!DNL Platform] Edge教程集成

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">为要引入的数据创建架构</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">为要引入的数据创建数据集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架构</a>上配置正确的身份和身份命名空间，以确保摄取的数据可以拼合到统一配置文件。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为配置文件</a>启用架构和数据集。</li>
    <li>使用以下方法之一将数据摄取到Experience [!DNL Platform]：</li>
        <ul>
           <li>体验[!DNL Platform] Web SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">教程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">清单</a></li>
                </ul>
            <li>体验[!DNL Platform] Mobile SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">教程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">清单</a></li>
                </ul></li>
            <li>Edge Network服务器API：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">教程</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">在体验[!DNL Platform]中创建区段。</a> 系统会自动确定评估区段是批处理（数据连接器）还是流式传输（Edge网络）。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">配置目标以将配置文件属性和受众成员身份共享到所需目标。</a></li>
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics]源连接器的标准工作流步骤将创建用于从[!DNL Analytics]“原样”中摄取数据的架构和数据集。 因此，前两个步骤由系统处理。 映射工作流需要创建自定义属性；因此，请完全遵循一系列步骤。
