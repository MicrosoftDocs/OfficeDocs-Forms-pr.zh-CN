---
title: 查看和取消阻止检测到具有潜在网络钓鱼并被阻止的的表单或用户
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms 允许自动计算机审阅主动检测表单和调查中的恶意敏感数据收集。 如果你是全局管理员和/或安全管理员，可以登录到 Microsoft 365 管理中心查看和取消阻止检测到具有潜在网络钓鱼和恶意目的被阻止的表单。
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951441"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>查看和取消阻止检测到具有潜在网络钓鱼并被阻止的的表单或用户

Microsoft Forms 允许自动计算机审阅主动检测表单中敏感数据的恶意收集，并临时阻止这些表单收集回复。 详细了解 [Microsoft Forms 和主动网络钓鱼防护](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)。

>[!Note]
>本文档中的步骤也适用于以前称为 Forms Pro 的 [Dynamics 365 客户语音](https://go.microsoft.com/fwlink/p?linkid=2128500)。 请注意，需要 Dynamics 365 客户语音许可证才能取消阻止 Dynamics 365 客户语音调查。 [了解详细信息](/dynamics365/customer-voice/help-hub)。

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>查看 Microsoft 365 Defender 门户中的警报

如果你是全局管理员或安全管理员，你将在 [Microsoft 365 Defender](https://security.microsoft.com/) 门户收到有关潜在网络钓鱼表单的警报，并可以对这些表单采取措施。

>[!Note]
> 如果你是全局管理员，你将收到组织的数据隐私消息，包括租户内创建的任何被检测到可能存在网络钓鱼而被阻止的表单的每日通知。 你可以通过查找 **Microsoft Forms 网络钓鱼通知**在[消息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)看到这些通知。 (如果未在**所有活动邮件**选项卡/视图中看到此通知，则可以在**已消除的邮件**选项卡/视图中找到此通知。) 对于每个通知，请选择**表单管理员审阅 URL**链接以查看被阻止的表单。  
  
为了使安全管理员也能够接收有关潜在网络钓鱼表单的通知，全局管理员需要为其分配[消息中心隐私读取者](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader)角色。 若要了解有关消息中心的详细信息，请参阅 [常见问题](/microsoft-365/admin/manage/message-center)。 另请参阅如何 [为数据隐私消息设置电子邮件首选项](/microsoft-365/admin/manage/message-center#preferences)。

1.  登录到 [Microsoft 365 Defender](https://security.microsoft.com/) 门户。

2.  选择**事件和警报** \> **警报**。 可能会看到关于 Forms 的以下一条或全部警告：
    
      - **用户已被限制共享表单和收集回复**
    
      - **表单已被标记并确认为网络钓鱼**
    
      - **表单因潜在的网络钓鱼尝试已被阻止**

3.  选择警报进行查看。 若要查看已标记的表单，请点击或单击右下角**管理警报**按钮旁边的三个点，然后选择**查看此表单**。
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="查看此表单选项":::

    >[!Tip]
    >详细了解 [Microsoft 365 中的警报策略](/microsoft-365/compliance/alert-policies)。

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>取消阻止表单或确认其网络钓鱼尝试

对于查看的每个表单，可以选择是取消阻止还是确认其为网络钓鱼。

### <a name="unblock"></a>取消阻止

如果你不认为表单有恶意企图，请选择**取消阻止**。

>[!Note]
>如果租户中的某人请求你取消阻止其表单，我们建议你要求其提供特定表单信息 (例如阻止的日期和时间、标题) 以便更有效地在管理中心识别通知。 由于通知每天发送一次，并且包括过去 24 小时内检测到的所有表单，因此用于识别表单的信息将非常有用。

### <a name="confirm-phishing"></a>确认网络钓鱼

如果你认为表单有恶意企图，请选择**确认网络钓鱼**。 该表单将被永久阻止，并且其所有者将无法再编辑或删除它。

选择**确认网络钓鱼**后，单击或点击**删除表单**以从租户中永久删除该表单。 我们强烈建议立即为租户中你认为已泄露的帐户重置密码。

>[!Tip]
>你对**确认网络钓鱼**的选择可帮助 Microsoft Forms 提高其检测准确度。 

## <a name="commonly-asked-questions"></a>常见问题

**当我查看被阻止的表单时，为什么我看不到取消阻止或确认网络钓鱼的选项？**

查看时，你可能看到对表单的阻止已解除。 这意味着在表单被阻止和查看表单之间，表单所有者删除了标记为潜在网络钓鱼的关键字。 在这种情况下，无需执行任何进一步的操作。

**如果表单已确认为网络钓鱼并被阻止，我能否将其删除？**

如果表单已确认为网络钓鱼并被阻止，请选择**删除表单**以将其从租户中删除。

**如果我对被阻止的表单不采取措施，会怎么样？**

如果选择不采取措施 (取消阻止表单或确认其网络钓鱼)，表单将一直被阻止。 表单所有者仍可编辑表单并删除标记为潜在网络钓鱼的关键字。

**如果我想编辑或删除表单中被阻止的内容，如何操作？**

如果你更喜欢编辑和/或删除被阻止的内容，可以生成一个共同创作页面，并作为共同作者管理表单。 为此，请单击你所查看的表单上方消息中的**打开一个共同创作页面**的链接。

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>删除被阻止的 Microsoft Forms 用户的限制

Microsoft Forms 会阻止反复尝试收集个人或敏感信息的用户分发表单和收集回复。 将通过[消息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)通知全局管理员这些被阻止的用户。 如果你认为阻止的用户没有恶意企图，并且他们的帐户是安全的，你可以执行以下步骤来取消阻止他们。

>[!Note]
>如果全局管理员为其分配了[邮件中心隐私读者](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader)角色，安全管理员也可以接收有关潜在网络钓鱼表单的通知。

1.  转到[消息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)并查找通知**预防/修复：Microsoft Forms 检测到潜在网络钓鱼**。

    >[!Note]
    >如果在**所有活动邮件**选项卡/视图中未看到此通知，则可以在**已消除的邮件**选项卡/视图中找到此通知。
 
    此通知包含租户中被阻止共享表单和收集回复的用户列表。

2.  单击通知中提供的链接以查看被阻止的用户。

3.  对于你认为没有恶意企图的每个用户，可以选择单击与该用户关联的**操作**列中的**取消阻止**链接。

    >[!Note]
    >如果你认为用户有恶意企图，则无需你执行进一步的操作。

    >[!Note]
    >移除限制可能需要 30 分钟或更长时间。

