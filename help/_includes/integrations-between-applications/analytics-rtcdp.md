---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# 将Adobe[!DNL Analytics]与实时客户数据[!DNL Platform]集成

{{analytics-description}}

{{real-time-cdp-description}}

将Adobe[!DNL Analytics]与Adobe实时客户数据[!DNL Platform] (Real-Time CDP)集成可以为希望增强其客户体验和营销工作的企业提供多种好处。 以下是一些主要优势：

+ **增强的受众定位和个性化**：设备和渠道上的精确营销，针对优化参与量身定制的消息。
+ **改进的登陆页面优化**：根据设备和行为定制体验，提高用户满意度和转化率。
+ **无缝受众激活**：利用客户配置文件通过首选渠道进行有效定位，并传递相关消息。

通过将Adobe[!DNL Analytics]与Real-Time CDP相结合，企业可以将营销工作提升到新的水平，提供个性化体验，提高客户参与度并优化各种数字接触点的转化。

<table>
    <thead>
        <tr>
            <th>Experience Cloud应用程序</th>
            <th>集成使用</th>
            <th>使用时间</th>
            <th>常见使用案例</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] 使用Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">体验[!DNL Platform]源连接器</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>推荐的方法适用于已实施Adobe[!DNL Analytics]并且希望以最快的方式将此数据摄取到Experience [!DNL Platform]以在实时客户档案中使用的客户。</li>
                <li>当数据收集开始后，实时客户档案的数据可用性可能为2-30分钟，并且数据湖的可用性最高可达90分钟。</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>通过用户界面启动的工作流非常简单。</li>
                <li>将用户界面映射到将[!DNL Analytics]属性和eVar复制到新的XDM字段。</li>
                <li>从Real-time Customer Profile和Customer历程[!DNL Analytics]中获取价值的最快方式。</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">体验[!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>建议新[!DNL Analytics]实施或想要实施长期策略时采用的方法。</li>
                <li>使用AEP Web SDK、AEP Mobile SDK或Edge Network服务器API，将数据直接从设备发送到Experience [!DNL Platform]。</li>
                <li>新客户或现有客户需要将[!DNL Analytics]数据可用性提供给实时客户档案，以支持相同和下一页个性化用例。</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>为收集用于支持用例的数据提供最高级别的控制。</li>
                <li>客户端数据可轻松映射到XDM字段。</li>
                <li>使Real-time Customer Profile能够更快地提供数据。</li>
            </ul>
        </td>
    </tr>            
</table>
