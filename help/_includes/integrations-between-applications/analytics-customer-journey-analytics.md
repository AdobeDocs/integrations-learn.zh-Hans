---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# 将Adobe[!DNL Analytics]与客户历程[!DNL Analytics]集成

{{analytics-description}}

{{customer-journey-analytics-description}}

将Adobe[!DNL Analytics]与客户历程[!DNL Analytics]集成提供了以下主要优点：

+ **对客户行为和偏好的全面洞察**。
+ **无缝跨渠道跟踪**&#x200B;以实现整体视图。
+ **统一数据和报表**&#x200B;以进行准确分析。
+ **增强了个性化**&#x200B;并提高了客户参与度。
+ **实时数据洞察**，用于Agile决策。

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
            <td rowspan="2">[!DNL Analytics] 和客户历程 [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">体验[!DNL Platform]源连接器</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>推荐的方法适用于已实施Adobe[!DNL Analytics]，并希望以最快的方式将此数据摄取到Experience [!DNL Platform]以在客户历程[!DNL Analytics]中使用的客户。</li>
                    <li>当数据收集开始后，客户配置文件的数据可用性可能介于2-30分钟之间，并且数据湖的可用性长达90分钟。</li>
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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">体验[!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>建议新[!DNL Analytics]实施或想要实施长期策略时采用的方法。</li>
                    <li>使用AEP Web SDK、AEP Mobile SDK或Edge Network服务器API，将数据直接从设备发送到Experience [!DNL Platform]。</li>
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
    </tbody>          
</table>
