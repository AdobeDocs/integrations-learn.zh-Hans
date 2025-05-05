---
title: 将 [!DNL Analytics] 和实时客户数据 [!DNL Platform] 与Experience [!DNL Platform] Edge教程集成
description: 了解如何使用AEP Web SDK、AEP Mobile SDK或Edge Network服务器API将Adobe [!DNL Analytics] 与实时客户数据 [!DNL Platform] 集成。
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="集成" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 2%

---

# 将Adobe[!DNL Analytics]和实时客户数据[!DNL Platform]与Experience [!DNL Platform] Edge教程集成

<ol>
    <li><a href="https://experienceleague.adobe.com/zh-hans?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">为要引入的数据创建架构</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为要引入的数据创建数据集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">在架构</a>上配置正确的身份和身份命名空间，以确保摄取的数据可以拼合到统一配置文件。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">为配置文件</a>启用架构和数据集。</li>
    <li>使用以下方法之一将数据摄取到Experience [!DNL Platform]：</li>
        <ul>
           <li>体验[!DNL Platform] Web SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">教程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">清单</a></li>
                </ul>
            <li>体验[!DNL Platform] Mobile SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">教程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">清单</a></li>
                </ul></li>
            <li>Edge Network服务器API：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">教程</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">在体验[!DNL Platform]中创建区段。</a>系统自动确定评估该区段是批处理（数据连接器）还是流式传输(Edge网络)。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=zh-Hans" _target="_blank" rel="noopener noreferrer">配置目标以将配置文件属性和受众成员身份共享到所需目标。</a></li>
</ol>

>[!NOTE]
>
>Adobe[!DNL Analytics]源连接器的标准工作流步骤将创建用于从[!DNL Analytics]“原样”中摄取数据的架构和数据集。 因此，前两个步骤由系统处理。 映射工作流需要创建自定义属性；因此，请完全遵循一系列步骤。
