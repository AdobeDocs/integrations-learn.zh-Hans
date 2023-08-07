---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 2%

---


# 集成Adobe [!DNL Analytics] 与客户历程 [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

集成Adobe [!DNL Analytics] 与客户历程 [!DNL Analytics] 提供以下主要优势：

+ **全面的见解** 顾客的行为和喜好。
+ **无缝的跨渠道跟踪** 以全面了解。
+ **统一的数据和报告** 以便进行准确分析。
+ **增强的个性化** 以及提高客户参与度。
+ **实时数据洞察** 用于敏捷决策。

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
            <td rowspan="2">[!DNL Analytics] 和客户历程 [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">体验 [!DNL Platform] 源连接器</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>为已实施Adobe的客户推荐的方法 [!DNL Analytics]，并希望以最快的方式将此数据摄取到Experience [!DNL Platform] 在客户历程中使用 [!DNL Analytics].</li>
                    <li>当数据收集开始后，客户配置文件的数据可用性可能介于2-30分钟之间，并且数据湖的可用性长达90分钟。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>通过用户界面启动的工作流非常简单。</li>
                    <li>将用户界面映射到复制 [!DNL Analytics] prop和eVar添加到新XDM字段。</li>
                    <li>从Real-time Customer Profile和Customer历程中获取价值的最快方式 [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">体验 [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>建议的新方法 [!DNL Analytics] 实施或希望实施长期策略的时间。</li>
                    <li>将数据直接从设备发送到Experience [!DNL Platform] 使用AEP Web SDK、AEP Mobile SDK或Edge Network服务器API。</li>
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
