---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---


# [!DNL Analytics] 和Audience Manager集成

{{analytics-description}}

{{audience-manager-description}}

通过转发Adobe启用此集成 [!DNL Analytics] 数据服务器端到Audience Manager，为Audience Manager提供了其主要的数据来源之一，即在线客户行为数据。 然后，此数据可以与其他数据（如第一方CRM数据或第三方合作伙伴数据）相结合，以创建丰富的客户区段。 此外，Audience Manager区段随后在响应中发送回网页，以供进一步访客分析。 这两个有价值的用例如下所述。

集成Adobe的主要优势 [!DNL Analytics] 和Audience Manager为：

+ **增强的分段**：合并Adobe [!DNL Analytics] 和Audience Manager数据，以在营销活动中获得精确、个性化的受众区段。
+ **统一的客户配置文件**：集成数据源以了解交互和行为，创建全面的客户档案。
+ **广告效果改进**：使用Adobe中的数据驱动定位优化广告 [!DNL Analytics] 和Audience Manager集成。
+ **数据驱动型决策**：通过详细的洞察和合并Adobe告知选择 [!DNL Analytics] 和Audience Manager数据。
+ **个性化体验**：定制您的内容和选件，使用这两个平台丰富客户在接触点之间的交互。

总体而言，此集成汇集了宝贵的数据和受众见解。 它使企业能够创建更有针对性和更相关的营销活动，同时加深对其客户偏好和行为的了解。

## 常见集成

<table>
    <thead>
        <tr>
            <th>Experience Cloud应用程序</th>
            <th>集成使用</th>
            <th>使用场合</th>
            <th>常见使用案例</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] 向Audience Manager发送数据</a>
            </td>
            <td>Adobe [!DNL Analytics] 启用了服务器端转发的标记扩展或AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>当您要发送Adobe时 [!DNL Analytics] 要Audience Manager的数据，用于创建可与其他Adobe Experience Cloud目标、基于人员的目标或Audience Manager支持的其他基于设备和自定义目标共享的区段。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>将区段共享到包含在中收集的行为属性的广告平台 [!DNL Analytics].</li>
                    <li>使用扩充区段 [!DNL Analytics] 创建高价值、跨渠道区段以用于网站定位的数据。</li>
                    <li>图层位于 [!DNL Analytics] 数据发送到通过哈希标识符（如电子邮件）加密的区段，以便在社交媒体平台中使用。</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager将数据发送回 [!DNL Analytics]</a>
            </td>
            <td>Adobe [!DNL Analytics] 启用了服务器端转发的标记扩展或AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>当您要将区段从Audience Manager共享到时 [!DNL Analytics] 以告知受众发现、分段和优化。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>在中使用包含来自第三方提供商的人口统计数据的Audience Manager区段 [!DNL Analytics] 报表。</li>
                    <li>在中使用包含来自广告服务器的促销活动数据的Audience Manager区段 [!DNL Analytics] 报表。</li>
                    <li>在中使用包含已载入CRM数据的Audience Manager区段 [!DNL Analytics] 报表。</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
