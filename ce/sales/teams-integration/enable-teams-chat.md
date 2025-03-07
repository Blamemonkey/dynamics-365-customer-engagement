---
title: "Enable or disable Teams chat in Sales Hub | MicrosoftDocs"
description: "Enable Teams chat to help users effectively collaborate on their sales records without having to leave the application."
ms.date: 05/24/2022
ms.topic: article
search.app: 
  - D365CE
  - Powerplatform
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Configure Microsoft Teams chat in Sales Hub (preview)

[!INCLUDE [cc-beta-prerelease-disclaimer](../../includes/cc-beta-prerelease-disclaimer.md)]

[!INCLUDE [preview-disclaimer](../../includes/preview-disclaimer.md)]

As an administrator, you can configure the ability for sellers to chat in Microsoft Teams from within the Sales Hub app and custom apps. This helps with effective collaboration on the sales records without having to leave the application.

> [!NOTE]
> Teams settings apply across all customer engagement apps. So, whether you enable the feature from Sales Hub or a custom app, it'll be enabled for all supported customer engagement apps.

When the feature is enabled, while working on sales records, sellers can start a new chat or link an existing chat to a record, and thus collaborate efficiently without switching context or leaving the application. Linking all the associated chats to a record can help sellers maintain all the chats related to the record in one place. You can also configure an optional introduction message that sellers can use to provide further context when collaborating on Teams.

This feature requires certain permissions to access Teams data. Review the [Permissions required](#permissions-required) and [Data security and privacy](#data-security-and-privacy) sections to know more.

## Permissions required

| **Permission**      | **Type**    | **What the app does with the permission**       |
|---------------------|-------------|-------------------------------------------------|
| Chat.ReadWrite.All  | Delegated   | Reads a user's chats and recent messages to display in the chat list.         |
| Directory.Read.All  | Delegated   | Reads the display names for user's teams and channels.     |
| Presence.Read.All   | Delegated   | Reads presence information for all users to be displayed on the user avatars in the chat list.    |
| User.Read.All       | Application | Reads the display name and licenses of users to validate whether the suggested participants have a Teams license assigned. This permission is used by the **Suggested chats & contacts** section in the chat list. The permission is set at the application level, because it's used by a background service for better performance. |
| User.ReadBasic.All  | Delegated   | Reads users' photos.  |

## Enable or disable Teams chat

1. In the Sales Hub app, select **Change area** ![Icon to change the work area](media/change-area-icon.png) in the lower-left corner, and then select **App Settings**.

2. Under **General Settings**, select **Chat and collaborate**.

3. Turn on the **Turn on Microsoft Teams chats inside Dynamics 365 (preview)** toggle.
    
    > [!IMPORTANT]
    > You must be a global administrator (tenant administrator) to provide the initial consent. After that, application administrators can enable the preview for other instances.

4. To set the chat title to be used as the record title by default, turn on the **Use record title as the default chat name for linked chats** toggle. Users can change the title if they want.

    :::image type="content" source="media/teams-settings.png" alt-text="Teams settings page showing these two toggles set to Yes.":::

5. Save the changes.

The preview is now enabled for all the customer engagement apps. You can open a record and verify whether you're able to view the chats and channels related to the record. More information: [Open Teams chats and channels related to a record](using-teams-chat-in-dynamics.md#open-teams-chats-and-channels-related-to-a-record)


## Add the Teams settings page to the sitemap of a custom app

1. Sign in to [Power Apps](https://make.powerapps.com/).

2. Select the environment, and then select **Apps**. 

3. Select your custom app, and then select **Edit**.

4. In the **App Designer**, edit the **Site Map**.

5. To add the Teams **Chat and collaborate** settings page, add a subarea component, and then from the **Type** list, select  **URL**.

6.  Copy the following value and paste it into the **URL** field:  
    ```/main.aspx?pagetype=control&controlName=MscrmControls.TeamsCollaborationAdmin.TeamsCollaborationAdmin```

7. Save and publish the changes.


## Enable Teams chat from Power Platform admin center

1. Sign in to [Power Platform admin center](https://admin.powerplatform.microsoft.com).

2. Go to the **Environments** tab, select an environment in which you want to enable Teams chat.

3. On the **Environments** page, select **Settings**.

4. On the **Settings** page, expand **Integration**, and then select **Teams integration settings**.

    :::image type="content" source="media/ppac-teams-chat.png" alt-text="Enable Teams chat from Power Platform admin center":::

5. On the **Microsoft Teams collaboration and chat** page, perform the following actions:
    
    1. Turn on the **Turn on Microsoft Teams chats inside Dynamics 365 (preview)** toggle.

    2. To set the chat title to be used as the record title by default, turn on the **Use record title as the default chat name for linked chats** toggle. Users can change the title if they want.

        :::image type="content" source="media/teams-settings.png" alt-text="Teams settings page showing these two toggles set to Yes.":::

6. Save the changes.

## Data security and privacy

The following data security and privacy considerations apply for Teams chat functionality in Dynamics 365:

- Dynamics 365 doesn't store any Teams data, except for the mapping between the record ID and the linked chat ID. No data from Teams is duplicated in Dynamics 365, unless the user manually adds it to the record notes or tasks.

- The communication between the applications is secured through TLS.

- Policies that apply both to Teams and Dynamics 365 are honored by the integration. For example, confidential files shared in a linked chat can only be accessed by permitted users. Similarly, a record shared in a Teams chat in Dynamics 365 can only be accessed if the user has permissions to view it.  

- The app requires certain permissions to start a chat, display suggested contacts, show presence, and so on. For more information, go to [What are the privileges and type of permissions required by the integration?](teams-in-dynamics-faq.md#what-are-the-privileges-and-types-of-permissions-required-by-the-integration).  


### See also

[Use Microsoft Teams chat in Sales Hub](using-teams-chat-in-dynamics.md)  
 
