---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# [!DNL Analytics]与Audience Manager集成

{{analytics-description}}

{{audience-manager-description}}

启用此集成(通过将Adobe[!DNL Analytics]数据服务器端转发到Audience Manager)，可为Audience Manager提供其主要数据源之一，即在线客户行为数据。 然后，此数据可以与其他数据（如第一方CRM数据或第三方合作伙伴数据）相结合，以创建丰富的客户区段。 此外，Audience Manager区段随后在响应中发送回网页，以供进一步访客分析。 这两个有价值的用例如下所述。

集成Adobe[!DNL Analytics]和Audience Manager的主要好处是：

+ **增强的分段**：将Adobe[!DNL Analytics]与Audience Manager数据相结合，在营销活动中形成精确、个性化的受众区段。
+ **统一客户配置文件**：集成数据源以了解交互和行为，创建全面的客户配置文件。
+ **广告效果提高**：通过Adobe[!DNL Analytics]中的数据驱动定位与Audience Manager集成，优化广告。
+ **数据驱动决策**：通过详细的分析、合并Adobe[!DNL Analytics]和Audience Manager数据告知选择。
+ **个性化体验**：定制您的内容和选件，使用两个平台丰富客户在接触点之间的交互。

总体而言，此集成汇集了宝贵的数据和受众见解。 它使企业能够创建更有针对性和更相关的营销活动，同时加深对其客户偏好和行为的了解。

## 常见集成

<table>
    <thead>
        <tr>
            <th>Experience Cloud应用程序</th>
            <th>集成使用</th>
            <th>使用时间</th>
            <th>常见使用案例</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics]将数据发送到Audience Manager</a>
            </td>
            <td>Adobe[!DNL Analytics]标记扩展或启用了服务器端转发的AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>当您想要将Adobe[!DNL Analytics]数据发送到Audience Manager以创建区段时，这些区段可以与其他Adobe Experience Cloud目标、基于人员的目标或Audience Manager支持的其他基于设备和自定义目标共享。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>将区段共享到广告平台，这些广告平台包含在[!DNL Analytics]中收集的行为属性。</li>
                    <li>使用[!DNL Analytics]数据扩充区段，以创建高价值的跨渠道区段用于现场定位。</li>
                    <li>将[!DNL Analytics]数据中的层传递到通过哈希标识符（如电子邮件）作为关键字的区段，以便在社交媒体平台中使用。</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager将数据发送回[!DNL Analytics]</a>
            </td>
            <td>Adobe[!DNL Analytics]标记扩展或启用了服务器端转发的AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>当您想要将区段从Audience Manager共享到[!DNL Analytics]以告知受众发现、分段和优化时。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>在[!DNL Analytics]报表中使用包含来自第三方提供商的人口统计数据的Audience Manager区段。</li>
                    <li>在[!DNL Analytics]报表中使用包含来自广告服务器的促销活动数据的Audience Manager区段。</li>
                    <li>在[!DNL Analytics]报表中使用包含已载入CRM数据的Audience Manager区段。</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
