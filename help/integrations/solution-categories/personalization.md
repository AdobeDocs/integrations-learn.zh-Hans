---
title: 大规模个性化的应用程序集成
description: 让个性化的体验成为每个时刻的一部分。
exl-id: 6d18813d-950c-40ae-8d5b-80bf389358fc
source-git-commit: 132c892723d29d415d07093ef8514ff8c9b7b1db
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 1%

---

# 大规模Personalization

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
      <td><strong>创建个性化的PDF文档</strong></td>
      <td>
        根据用户生成要签名的通信文档
        选择/首选项。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            基于来自AEM的数据提供动态生成的NDA
            提交Forms以进行签名
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-acrobat-sign.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Forms和签名</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>数据分析和报告</strong></td>
      <td>
        分析数字体验中的行为数据<br />使用Adobe
        客户历程中Analysis Workspace的[!DNL Analytics]行为数据
        [!DNL Analytics]。
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
          >[!DNL Analytics]和客户历程[!DNL Analytics]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        个性化活动的报表<br />分析优化
        利用Adobe [!DNL Target]和测试结果（包括A/B测试）
        通过Adobe [!DNL Analytics]生成综合报告。
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
        利用动态内容个性化电子邮件投放
        Adobe [!DNL Target]的功能。
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
        使用Audience Manager区段在Real-Time CDP中创建受众，以
        用于个性化和再营销策略。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            对执行匿名数字受众定位和个性化
            网站、移动应用程序或支持的广告渠道上的
          </li>
          <li>
            根据优化登陆页面和预身份验证体验
            已知设备和行为特征
          </li>
          <li>
            利用Audience Manager第三方数据网络进一步实现
            优化和扩展受众以进行定位
          </li>
          <li>将Audience Manager区段共享到RTCDP</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/aam/aam-rtcdp.md"
          target="_blank"
          rel="noopener noreferrer"
          >Audience Manager和实时客户数据[!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        使用[!DNL Analytics]数据创建受众以用于个性化或
        再营销策略。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            在设备上执行数字受众定位和个性化，或
            支持的广告渠道。
          </li>
          <li>
            优化已知的客户登陆页面和匿名体验
            基于设备和行为属性。
          </li>
          <li>将受众激活到已知渠道，如电子邮件和短信。</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics]和实时客户数据[!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>个性化Web体验</strong></td>
      <td>
        通过有效地自定义单页应用程序(SPA)体验
        将AEM Headless与Adobe [!DNL Target]结合使用。
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
          >AEM Headless和[!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        通过有效利用AEM Sites提供量身定制的网站体验
        和Adobe [!DNL Target]进行个性化。
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>AEM网站个性化。</li>
          <li>A/B测试变体。</li>
          <li>基于用户行为的行为定位。</li>
          <li>通过拼接来自多个系统的用户数据，提供360度客户视图，实现已知用户个性化。</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Sites和[!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>个性化数字体验</strong></td>
      <td>
        使用实时客户配置文件和集中管理的[!DNL Platform]区段
        个性化跨Web、移动和其他数字渠道的消息传递
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
          >实时客户数据[!DNL Platform]和[!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>增强商机拓展</strong></td>
      <td>
        使用实时客户配置文件和集中管理的[!DNL Platform]区段
        个性化跨Web、移动和其他数字渠道的消息传递
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
          >实时客户数据[!DNL Platform]和[!DNL Target]</a
        >
      </td>
    </tr>
  </tbody>
</table>
