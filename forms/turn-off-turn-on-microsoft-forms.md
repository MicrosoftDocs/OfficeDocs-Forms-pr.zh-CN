---
title: 关闭或打开 Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 本文介绍了 Microsoft 365 管理员如何为整个组织或组织中特定人员关闭或打开 Microsoft Forms。
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951403"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>关闭或打开 Microsoft Forms

默认情况下，将为组织中的每个人启用 [Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8)。 如果你是[管理员](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504)，你可以[设置 Microsoft Forms](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240)，然后为整个组织或仅特定人员将其关闭或再次打开。

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>为组织中的每个人关闭 Microsoft Forms

1.  登录到[Microsoft Azure](https://portal.azure.com/)。

2.  在左窗格中，单击**Azure Active Directory**。

3.  单击 **企业应用程序**。

4.  导航到所需的服务，然后对**应用程序类型**\>**CollabDBService**和**Microsoft 应用程序** \> **MicrosoftForms** 重复步骤 5-7。 
    
      - 在**应用程序类型**下拉列表下的搜索字段中，键入 **CollabDBService**。 在搜索结果列表中选择**CollabDBService**。
    
      - 在**应用程序类型**下拉列表中，选择**Microsoft 应用程序**。 在**应用程序类型**下拉列表下的搜索字段中，键入 **Microsoft Forms**，然后在搜索结果列表中选择**Microsoft Forms**。

5.  在**管理**下，单击**属性**。

6.  对于选项**为用户启用登录？**，选择**否**。

7.  单击“**保存**”。

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>为组织中特定人员关闭 Microsoft Forms

1.  使用你的 Microsoft 365 工作或学校帐户作为全局管理员登录。[了解如何登录](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4)。

2.  在 Microsoft 365 管理中心中，选择**用户** \> **活动用户**。

3.  选中要关闭其 Microsoft Forms 的人的姓名旁边的框。

4.  在功能区上，单击**管理产品许可证**。

5.  在打开的帐户表单中，在**许可证和应用**选项卡上，展开应用程序部分并向下滚动到 Microsoft Forms 选项。 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Microsoft 365 中心的帐户选项表单":::

6.  清除此框以关闭 Microsoft Forms。 若要将其打开，请选中该复选框。

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text=" Microsoft Forms 切换":::

     > [!Note]
     > [检查此列表](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e)以查看你是否具有包含 Microsoft Forms 的 Office 许可证。 如果已列出你的许可证，则需要清除 Microsoft Forms 复选框以完全关闭用户访问。

7.  在**应用**列表底部，单击**保存更改**。

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>我打开了 Microsoft Forms，但组织成员仍然无法访问它

在 Microsoft Azure 中检查以下设置，以确保 Microsoft Forms 已启用：

1.  登录到[Microsoft Azure](https://portal.azure.com/)。

2.  在左窗格中，单击**Azure Active Directory**。

3.  单击 **企业应用程序**。

4.  导航到所需的服务，然后对**应用程序类型**\>**CollabDBService**和**Microsoft 应用程序** \> **MicrosoftForms** 重复步骤 5-7。 
    
      - 在**应用程序类型**下拉列表下的搜索字段中，键入 **CollabDBService**。 在搜索结果列表中选择**CollabDBService**。
    
      - 在**应用程序类型**下拉列表中，选择**Microsoft 应用程序**。 在**应用程序类型**下拉列表下的搜索字段中，键入 **Microsoft Forms**，然后在搜索结果列表中选择**Microsoft Forms**。

5.  在**管理**下，单击**属性**。

6.  对于选项**为用户启用登录？**，选择**是**。

7.  单击“**保存**”。

    >[!Note]
    >必须启用 SharePoint 服务以便组织成员可以访问 Microsoft Forms。

## <a name="feedback-for-microsoft-forms"></a>有关 Microsoft Forms 的反馈

欢迎提出宝贵意见\! 若要发送有关 Microsoft Forms 的反馈，请转到表单的右上角，然后选择**更多窗体设置** ![更多选项按钮](./media/image2.png) \> **反馈**。

