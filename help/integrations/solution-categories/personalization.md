---
title: 大规模个性化
description: 让个性化的体验成为每个时刻的一部分。
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 1%

---


# 大规模个性化

在当今高度竞争和数字化驱动的格局中，客户期待着根据其独特偏好和需求定制的体验。 利用Adobe Experience Cloud的功能，我们可以收集和分析广泛的客户数据，为行为、兴趣和偏好提供宝贵的见解。 这种深入的了解有助于在各种接触点之间交付个性化体验，确保进行有意义、引人入胜的交互。 利用Adobe Experience Cloud的强大功能释放出个性化的全部潜力，建立更强大的客户关系，培养忠诚度，并驱动业务增长。

<table>
 <thead>
    <tr>
      <th>用例</th>
      <th>描述</th>
      <th>示例</th>
      <th>应用程序</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>创建个性化PDF文档</strong></td>
      <td>
        根据用户选择/偏好设置生成要签名的通信文档。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            根据AEM Forms提交以供签名的数据提供动态生成的NDA
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-acrobat-sign.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Forms and Sign</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>数据分析和报告</strong></td>
      <td>
        分析来自数字体验的行为数据 <br />使用Adobe
        [!DNL Analytics] Analysis Workspace中的行为数据客户历程
        [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>分析顶部/底部转换路径</li>
          <li>分析渠道参与和转化</li>
          <li>了解最常查看的内容</li>
          <li>了解热门产品类别和产品</li>
          <li>
            执行工具使用分析以优化自助服务体验
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] 和客户历程 [!DNL Analytics]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        个性化活动报表<br />利用Adobe分析优化测试结果，包括A/B测试 [!DNL Target] 通过Adobe生成全面的报告 [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>在富分析报表中显示A/B测试结果</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] 和 [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>个性化电子邮件投放</strong></td>
      <td>
        利用Adobe功能，使用动态内容个性化电子邮件投放 [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>向客户电子邮件添加个性化优惠</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/campaign//campaign-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Campaign] 和 [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2">
        <strong>展开个性化和广告平台的受众</strong>
      </td>
      <td>
        在Real-Time CDP中使用Audience Manager区段创建受众，以用于个性化和再营销策略。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            在网站、移动应用程序或支持的广告渠道上执行匿名数字受众定位和个性化
          </li>
          <li>
            根据已知设备和行为特征优化登陆页面和预身份验证体验
          </li>
          <li>
            利用Audience Manager的第三方数据网络，进一步细化和扩展用于定位的受众
          </li>
          <li>将Audience Manager区段共享到RTCDP</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/aam/aam-rtcdp.md"
          target="_blank"
          rel="noopener noreferrer"
          >Audience Manager和实时客户数据 [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        使用 [!DNL Analytics] 用于创建受众以用于个性化或再营销策略的数据。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            在设备或支持的广告渠道上执行数字受众定位和个性化。
          </li>
          <li>
            根据设备和行为属性优化已知的客户登陆页面和匿名体验。
          </li>
          <li>将受众激活到已知渠道，如电子邮件和短信。</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] 和实时客户数据 [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>个性化Web体验</strong></td>
      <td>
        通过有效地将SPA Headless与Adobe结合使用，自定义单页应用程序(AEM)体验 [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>SPA和移动应用程序个性化</li>
          <li>个性化API响应。</li>
          <li>[!DNL Target]ed内容交付。</li>
          <li>A/B测试变体。</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM无头和 [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        通过有效利用AEM Sites和Adobe提供量身定制的网站体验 [!DNL Target] 进行个性化。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>AEM网站个性化。</li>
          <li>个性化网站内容。</li>
          <li>优化用户体验。</li>
          <li>A/B测试变体。</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Sites和 [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>个性化数字体验</strong></td>
      <td>
        使用实时客户配置文件并集中管理 [!DNL Platform] 区段，用于在Web、移动和其他数字渠道之间个性化消息传递
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>已知访客的内容个性化</li>
          <li>提高忠诚度注册和参与率</li>
          <li>识别面临客户流失风险的客户并与他们互动</li>
          <li>实时选件个性化</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >实时客户数据 [!DNL Platform] 和 [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>增强商机拓展</strong></td>
      <td>
        使用实时客户配置文件并集中管理 [!DNL Platform] 区段，用于在Web、移动和其他数字渠道之间个性化消息传递
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>已知访客的内容个性化</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >实时客户数据 [!DNL Platform] 和 [!DNL Target]</a
        >
      </td>
    </tr>
  </tbody>
</table>
