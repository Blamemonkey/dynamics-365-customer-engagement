---
title: Configure the ability to use suggested contacts when starting a Teams chat
description: Learn how to configure the ability to use suggested contacts.
ms.date: 05/25/2022
ms.topic: article
ms.service: dynamics-365-sales
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Configure the ability to use suggested contacts (preview)

[!INCLUDE [cc-beta-prerelease-disclaimer](../../includes/cc-beta-prerelease-disclaimer.md)]

[!INCLUDE [preview-disclaimer](../../includes/preview-disclaimer.md)]

As an administrator, you can enable the suggested contacts to be displayed when a seller starts a new linked chat. It helps the sellers to quickly find the right coworkers to collaborate with.

> [!NOTE]
> For the case record type, there are two types of contact suggestions: AI and rules-based. Other record types enabled for linked chats may only have rules-based suggestions.

**To turn on the suggested contacts capability for a record type**:

1. In the Sales Hub app, select **Change area** ![Icon to change the work area](media/change-area-icon.png) in the lower-left corner, and then select **App Settings**.

2. Under **General Settings**, select **Chat and collaborate**.

3. Under **Link chats to Dynamics 365 records**, select the record type (for example, Lead).

4. In the settings panel, turn on the **Rules-based suggested contacts** toggle.

    :::image type="content" source="media/lead-configure-suggest-contact.png" alt-text="Settings page to turn on or off the suggested contacts feature.":::

5. In the **Update rules for suggesting contacts** section, reorder or disable the rules for suggesting contacts. Users will see the suggestions in the order you choose.

    - To reorder the rules, hover over a rule, and then select the up or down arrow to move the rules up or down respectively.
    - To disable a rule, hover over a rule, and then select :::image type="icon" source="media/suggested-contacts-rule-disable.png" border="false":::. When the rule is disabled, :::image type="icon" source="media/suggested-contacts-rule-disabled.png" border="false"::: is displayed when you hover over the disabled rule.

    :::image type="content" source="media/suggested-contacts-rules.png" alt-text="Reorder or disable the rules for suggested contacts.":::

6. Select **Save**.

### See also

[Enable or disable Microsoft Teams chat in Sales Hub](enable-teams-chat.md)   
[Use Microsoft Teams chat in Sales Hub](using-teams-chat-in-dynamics.md)
