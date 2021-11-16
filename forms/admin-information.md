---
title: 管理员信息
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 本文解答了有关 Microsoft Forms 管理员信息的常见问题。
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951433"
---
# <a name="admin-information"></a>管理员信息

## <a name="getting-started"></a>入门

**如何关闭或打开 Microsoft Forms？**

默认情况下，将为组织中的每个人启用 Microsoft Forms。 Microsoft 365 IT 管理员可以在 Microsoft 365 管理中心的**用户管理**选项卡下关闭 Microsoft Forms。有关详细信息，请参阅[设置 Microsoft Forms](set-up-microsoft-forms.md)以及[关闭或打开 Microsoft Forms](turn-off-turn-on-microsoft-forms.md)。

**如何仅允许组织中特定人员访问 Microsoft Forms？**

管理员可以更改组织中特定人员的访问权限。 请参阅 [Microsoft Forms 中的管理员设置](administrator-settings-microsoft-forms.md)。

## <a name="data-storage"></a>数据存储

**Microsoft Forms 的数据存储在何处？**

Microsoft Forms 的数据存储在美国的服务器上，但位于欧洲的租户数据除外。 位于欧洲的租户数据存储在欧洲的服务器上。

## <a name="user-activity"></a>用户活动

**如何查看组织中人员在 Microsoft Forms 中进行的活动？**

可以在 [Microsoft 365 安全中心](https://security.microsoft.com/?rfr=OfficeScc)审核日志中查看 [Microsoft Forms 活动](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities)。 详细了解 [Office 365 中的审核 (适用于管理员)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906)。

## <a name="user-account-information"></a>用户帐户信息

**如何检查用户帐户是否已被"硬删除"？**

1. 管理员可以登录到 [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer)。

2. 在顶部搜索框中，粘贴以下 URL：

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*用户电子邮件* = 已离开组织的表单所有者和/或其帐户已被禁用的表单所有者的电子邮件地址。

3. 单击**运行查询**。

如果查询中返回了要查找的帐户信息，则意味着该帐户已被软删除且在 30 天期限内。 全局管理员可以使用上述转移方法转移已被软删除帐户所拥有的表单。

如果查询中未返回要查找的帐户信息，则意味着该帐户仍存在于 Office 365 租户中，或者已在 30 天以前被删除。 如果帐户在 Office 365 租户中存在或处于禁用状态，则全局管理员可以转移该帐户拥有的表单。 如果该帐户已从 Office 365 租户中被"硬删除"，则全局管理员将无法转移该帐户所拥有的表单。 这些表单也不可恢复。

**即使用户帐户离开我的组织，用户数量和存储的数据量是否有限制？**

目前，只要其帐户的预配在组织的联机服务协议中，保留其数据的用户数没有限制。 也不限制为用户帐户存储的数据量。

**如果删除了所有者的 Microsoft Forms 许可证，或者用户已从租户 (Azure AD) 中被删除或禁用，表单数据会发生什么情况？**

如果所有者许可证已被删除或所有者的帐户已被禁用，则用户帐户存储的数据量不会发生变化。

如果从租户 (Azure AD) 中删除了用户帐户，则所有与帐户相关的数据将在删除用户的 30 天后被删除。

## <a name="form-ownership-transfer"></a>表单所有权转移

**表单的原始所有者不再在我的组织中。如何转移其表单的所有权？**

若要转移已离开组织的人员的表单，必须满足以下要求：

  - 你是组织的全局管理员，并且拥有有效的 Forms 许可证。

  - 要转移其表单的员工的账户已被删除或禁用。

  - 在帐户删除后 30 天内转移表单。

> [!Note]
> 从已禁用（且未删除）的帐户转移表单所有权没有时间限制。

1. 如果满足所有要求，你可以转移表单所有权。 在浏览器的地址栏中，将现有 URL 替换为以下内容：

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*用户电子邮件* = 已离开组织的表单所有者和/或其帐户已被禁用的表单所有者的电子邮件地址。
   > 例如，如果表单所有者 ("Jason Fabian") 已离开组织 ("Contoso") ，你的解决方法 URL 将如下所示： `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. 你现在可以访问前员工的表单。 在要转移的表单中，单击**更多表单操作**![更多选项按钮](./media/image2.png) ，然后选择**移动**。

   >[!Note]
   >如果你想将表单的所有权转移给组织中当前处于活动状态的员工，可以将其移动到他们所属的组。 如果你不是该组的成员，则必须加入此组才能执行转移。 表单所有权转移完成后，可以选择退出组。

**当我尝试转移表单的所有权时，为什么会收到错误？**

如果收到错误消息，以下任何一项都可能会阻止你转移所有权：

|错误消息|说明|
| --- | --- |
| ***我们无法访问此页面***<br/><br/>表单所有者仍具有活动帐户。 | 表单的所有者仍具有活动的 Forms 许可证和帐户。 |
| ***我们无法访问此页面***<br/><br/>请确保正确输入了电子邮件地址，且表单所有者帐户不是在 30 天以前被删除。 | 电子邮件地址拼写不正确和/或表单所有者的帐户在 30 天之前被删除。 |
| ***我们无法访问此页面***<br/><br/>请确保已正确输入电子邮件地址，然后重试。 | 电子邮件地址缺失或拼写错误。 |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Outlook 或 PowerPoint 中的表单使用情况

**我组织中的人员无法向 Outlook 电子邮件中添加投票。如何解决此问题？**

需要启用 Outlook **新式验证**设置，以确保组织成员可以[在 Outlook 中创建投票](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0)。

1. 使用你的工作或学校帐户登录 [https://admin.microsoft.com](https://admin.microsoft.com/)。

2. 选择**设置** \> **组织设置**。

   >[!Note]
   > 如果看不到**设置**选项，请在左侧窗格中选择![更多选项按钮](./media/image2.png)**显示全部**。

3.  选择**新式验证**。

4.  选中**为 Outlook 2013 for Windows 及更高版本启用新式身份验证（推荐）** 选项。

详细了解新式和 [多重身份验证](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide)，以及如何对其进行设置并向组织推出。

**我不想为整个阻止部署 Office 加载项。我的组织成员是否仍可以使用适用于 PowerPoint 的 Forms 加载项？**

是的，可以使用[集中部署](/office/dev/add-ins/publish/centralized-deployment)来仅部署适用于 PowerPoint 的 Forms 加载项。

1.  使用你的工作或学校帐户登录 [https://admin.microsoft.com](https://admin.microsoft.com/)。

2.  选择**设置** \> **加载项**。

    >[!Note]
    >如果看不到**设置**选项，请在左侧窗格中选择![更多选项按钮](./media/image2.png)**显示全部**。

3.  在**加载项**列表中，选择 **Forms**。

4.  在**编辑 Forms**窗格中的**分配用户**下，选择**所有人**。

5.  选择 **“保存”**。


## <a name="forms-and-anti-phishing"></a>表单和防钓鱼

**对于租户内表单中的网络钓鱼和潜在恶意意图，我该怎么办？**

在 Microsoft Forms 中，我们启用自动计算机审阅，以主动检测表单中对敏感数据的恶意收集，并临时阻止这些表单收集回复。

详细了解 [Microsoft Forms 和主动网络钓鱼防护](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)。

如果你是全局管理员和/或安全管理员，可以登录到 Microsoft 365 管理中心 [admin.microsoft.com](https://admin.microsoft.com/) 并转到[消息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)。  在此处，你将获得任何以及所有被阻止表单的每日摘要。 对于列出的每个表单，你可以选择是取消阻止还是确认其为网络钓鱼尝试。 详细了解如何[查看和取消阻止被检测为潜在网络钓鱼并被阻止的表单或用户](review-unblock-forms-users-detected-blocked-potential-phishing.md)。
