---
title: 设置 Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 了解 Microsoft 365 管理员如何控制 Microsoft Forms 在组织中如何使用。 此外，了解安全性和合规性问题的答案，例如 Microsoft Forms 数据存储在何处。
ms.openlocfilehash: abee1557f379f646b277866f32fc0640c0b643cd
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951405"
---
# <a name="set-up-microsoft-forms"></a>设置 Microsoft Forms


## <a name="overview"></a>[概述](#tab/overview)

Microsoft Forms 允许用户快速而轻松地创建自定义测验、调查、问卷、注册等。 创建测验或表单后，甚至可以在移动设备上使用任何 Web 浏览器来邀请其他人作答。 提交结果后，可以使用内置的分析来评估这些回答内容。 可以轻松地将表单数据（例如，测验结果）导出为 Excel 进行进一步的分析或评分。

若要了解详细信息，请参阅[什么是 Microsoft Forms？](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) 或者，请参阅我们的[Microsoft 365 博客文章](https://go.microsoft.com/fwlink/?linkid=852256)以了解 Microsoft Forms。

>[!Note]
>Microsoft Forms 已正式向 Office 365 教育版客户、Microsoft 365商业应用版客户和具有 Microsoft 帐户（Hotmail、Live 或 Outlook.com）的客户提供。

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="预览表单在移动设备上的外观。":::

## <a name="configure"></a>[配置](#tab/configure)

Microsoft 365 管理员可通过以下任务控制 Microsoft Forms 在组织中如何使用：

<table>
<thead>
<tr class="header">
<th><strong>管理任务</strong></th>
<th><strong>说明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>关闭或打开 Microsoft Forms</strong></td>
<td>默认情况下，Microsoft Forms 为你的组织启用。 你可以随时<a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">关闭它</a>。</td>
</tr>
<tr class="even">
<td><strong>为组织中的单个人员关闭 Microsoft Forms</strong></td>
<td>当为特定人员关闭 Microsoft Forms 时，他们将不能使用它，并且 <strong>Forms</strong> 磁贴不会在 Microsoft 365 应用启动器或主页中显示。  了解如何 <a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">为特定人员关闭表单</a>。 </td>
</tr>
<tr class="odd">
<td><strong>为 Microsoft Forms 设置 Azure Active Directory 条件访问</strong></td>
<td><p>若要为 Microsoft Forms 设置条件访问策略，请查阅 <a href="/azure/active-directory/conditional-access/">Azure AD 条件访问文档</a>，并在<strong>云应用</strong>分配中包括<strong>Microsoft Forms</strong>。</p>
<p><strong>注意：</strong>如果在为 Microsoft Forms 设置条件访问后仍阻止你组织的用户，请确保 SharePoint Online 和 Exchange Online 也通过条件访问被授予了访问权限。 <a href="/azure/active-directory/conditional-access/conditional-access-for-exo-and-spo">了解详细信息</a>。</p></td>
</tr>
<tr class="even">
<td><strong>控制外部共享设置、记录组织中人员的姓名和/或保护表单免受钓鱼攻击</strong></td>
<td><p>在 Microsoft 365 管理中心中，你可以：</p>
<ul>
<li><p>控制是否允许外部用户与组织的用户协作处理表单或测验。</p></li>
<li><p>选择是否捕获组织中的填写表单的人的姓名。</p></li>
<li><p>关闭或打开表单上的自动网络钓鱼检测。</p></li>
</ul>
<p>详细了解这些 <a href="https://support.microsoft.com/office/administrator-settings-for-microsoft-forms-48161c55-fbae-4f37-8951-9e3befc0248b">管理员设置</a>。</p></td>
</tr>
<tr class="odd">
<td><strong>允许用户将表单插入 PowerPoint</strong></td>
<td><ol type="1">
<li><p>登录到 <a href="https://admin.microsoft.com/">https://admin.microsoft.com</a>。</p></li>
<li><p>单击<strong>设置&gt;</strong><strong>设置</strong>。</p></li>
<li><p>在<strong>设置</strong>页上的<strong>服务</strong>选项卡下，单击<strong>用户拥有的应用和服务</strong>。</p></li>
<li><p>选中<strong>允许用户访问 Office 应用商店</strong>选项，以允许用户将表单插入 PowerPoint。</p></li>
</ol>
<blockquote>
<p>请注意，可能需要几个小时更改才能生效。 <a href="/office365/admin/manage/manage-deployment-of-add-ins>Learn more</a>.</p>
</blockquote></td>
</tr>
</tbody>
</table>


## <a name="security--compliance"></a>[安全性与合规性](#tab/security)

如果你的公司在内容安全性和数据使用方面有需要符合的法律、法规和技术标准，那么本节内容再合适不过。

**Microsoft Forms 的数据存储在何处？**

Microsoft Forms 数据存储在位于美国和欧洲的服务器上。 所有数据都位于美国，但 2017 年 5 月之后开始使用 Microsoft Forms 的欧洲租户除外。 其数据存储在欧洲的数据库中。

**Microsoft Forms 是否合规？**

自 2018 年 5 月起，Microsoft Forms 已满足 GDPR 合规性要求。 有关详细信息，请参阅[符合 GDPR 的 Microsoft 365 数据主体请求](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json)。

**FERPA 和 BAA 保护是否部署到位？**

Microsoft Forms 符合 [FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) 和 [BAA 保护标准](https://www.microsoft.com/TrustCenter/Compliance/HIPAA)。

*即使用户帐户离开我的组织，用户数量和存储的数据量是否有限制？*

目前，只要其帐户的预配在组织的联机服务协议中，为其保留数据的用户数没有限制。 也不限制为用户帐户存储的数据量。

*表单的原始所有者已不在我的组织中，并且/或者其 Microsoft Forms 许可证已删除。与其创建的表单关联的数据会发生什么情况？*

从租户（Azure AD）中删除用户帐户30 天后，将删除所有与帐户相关的数据。

## <a name="faq"></a>常见问题

**可以使用 Microsoft Forms 进行哪些用途？**

Microsoft Forms 是一款简单而轻量型的应用，可让你轻松创建调查、测验和投票。 在教育机构中，它可用于创建测验、收集教师和家长的反馈，或规划课堂和教职员工活动。 在商业组织中，它可用于收集客户反馈、衡量员工满意度、改进产品或业务、或组织公司活动。

**谁可以使用 Microsoft Forms？**

任何拥有 Microsoft 帐户 (Hotmail、Live 或 Outlook.com) 的人都可以免费使用 Microsoft Forms。 以下 Office 365 教育版和 Microsoft 365 商业应用版客户也可使用 Microsoft Forms：

Office 365 教育版

  - Office 365 A1 Plus

  - Office 365 A5

  - 在停用前已购买 Office 365 教育版 E3 的现有客户

Microsoft 365 商业应用版

  - Microsoft 365 商业基础版

  - Microsoft 365 商业标准版

  - Microsoft 365 商业高级版

  - Microsoft 365 企业应用版

  - Microsoft 365 企业版 E1、E3 和 E5 计划

  - 在停用前已购买 Office 365 企业版 E4 的现有客户

登录到 [forms.office.com](https://forms.office.com/) 并开始创建调查、测验和投票。

**没有 Microsoft 365 帐户的人可以在 Microsoft Forms 上提交调查或测验吗？**

Microsoft Forms 作者可以切换其设置，以允许组织外部的用户回复他们的调查或测验。 在这种情况下，用户将匿名提交回复。 如果想要查看谁填写了你的调查或测验，可以要求调查者填写他们的姓名作为问卷的一部分。

**可以创建的表单数和每个表单可以接收的回复数的上线是多少？**

Office 365 教育版和 Microsoft 365 商业应用版客户最多可以创建 200 个表单，每个表单最多可接收 50000 个回复。 具有 Microsoft 帐户 (Hotmail、Live 或 Outlook.com) 的 Microsoft Forms 用户最多可以创建 200 个表单，付费帐户的每个表单最多可以接收 1000 个回复，免费帐户的每个表单最多可以接收 200 个回复。 详细了解 [表单、问题、回复和 Forms 中的字符限制](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea)。

如果需要更多回复，我们建议将现有回复导出到 Excel 工作簿，然后从调查或测验中清除这些回复。 这将使你能够在清除后收集更多回复。

**Microsoft Forms 可以使用哪些 Web 浏览器？**

Microsoft Forms 针对 Internet Explorer 11、Edge、Chrome (最新版本)、Firefox (最新版本)、Android 版 Chrome (最新版本) 和 iOS 上的 Safari (最新版本) 进行了优化。

**Microsoft Forms 适用于哪些语言？**

请参阅 Microsoft Forms [支持的语言](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac)和[语言设置](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27)。

**Microsoft Forms 将取代 Microsoft InfoPath 吗？**

否。 Microsoft InfoPath 是一种用于创建可启用自动化工作流的可自定义表单的解决方案，而 Microsoft Forms 是一款用于通过调查和测验快速收集信息的基本轻型应用。

Microsoft InfoPath 将由 SharePoint 列表、Flow 和 PowerApps 取代，这些新式解决方案将用于数字化传统公司表单、自动化工作流和转换业务流程。 [了解详细信息](https://products.office.com/business/business-process-automation)。

**可以去哪里提交产品 Bug 或功能请求等反馈？**

欢迎提出宝贵意见\! 若要发送有关 Microsoft Forms 的反馈，请转到表单的右上角，然后选择**更多表单设置** ![更多选项按钮](./media/image2.png)\>**反馈**。

>[!Note]
>有关详细信息，请参阅 [有关 Microsoft Forms 的常见问题解答](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c)。

