---
title: "Use Teams chat in Customer Service | Microsoft Docs"
description: "Learn how to use the Teams chat functionality in Dynamics 365 Customer Service and Dynamics 365 Customer Service workspace."
ms.date: 03/18/2022
ms.topic: article
author: lalexms
ms.author: laalexan
manager: shujoshi
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365CS
ms.custom: 
  - dyn365-customerservice
---

# Use Teams chat in Customer Service (preview)

> [!IMPORTANT]
> [!INCLUDE[cc-preview-feature](../includes/cc-preview-feature.md)]
>
> [!INCLUDE[cc-preview-features-definition](../includes/cc-preview-features-definition.md)]
>
> [!INCLUDE[cc-preview-features-expect-changes](../includes/cc-preview-features-expect-changes.md)]
>
> [!INCLUDE[cc-preview-features-no-ms-support](../includes/cc-preview-features-no-ms-support.md)]


As an agent, you can chat in Microsoft Teams from within Dynamics 365 Customer Service Hub, Customer Service workspace, and any custom app. While working on customer records, you can start a new chat or link an existing chat to a record, and thus collaborate efficiently without switching context or leaving the application. Linking all the associated chats to a record can help you maintain all the conversations related to the record in one place. 

> [!NOTE]
> This feature must first be enabled by an administrator, and you must have certain permissions to access Teams data. More information: [Configure Teams chat in Customer Service](configure-teams-chat.md)

## Agent overview of key features for Teams chat

The following image displays the key features of the agent Teams chat experience.

 > [!div class="mx-imgBorder"] 
 > ![Agent view of the Microsoft Teams chat experience in Dynamics 365 Customer Service.](media/teams-chat-agent-overview.png "Agent view of the Microsoft Teams chat experience")

The following legend describes the numbered callouts in the above image.

|Number |Feature | Description |
|-------|-----------|-----------|
| 1 | New chat | Create chats that aren't associated with any Dynamics 365 records.  |
| 2 | Filter |  Filter chats by name. |
| 3 | Chats linked to other records | Chats that are associated with other Dynamics 365 records that the current user is a part of. Users can prioritize responses to these chats over other chats. |
| 4 | New linked chat | Start a new chat that is linked with the record. These chats can only be viewed in Dynamics 365 by the chat participants. |
| 5 | Other chats | Chats that aren't linked to any records or started from Teams. |
| 6 | Chat control | Allows users to multi-task across chats. |
| 7 | Basic Teams functions | Format, use emojis, use gifs, set delivery options, attach files. |
| 8 | Add/remove participants | Select who participates in the chat and who doesn't. |


## Open Teams chats that are related to a record

You can open any Dynamics 365 Customer Service record and select the **Teams chats and channels integration** icon. The **Teams chats (preview)** panel opens with the following sections in the **Chat** tab:  
- Chats linked to the record: Lists Teams chats that either you’ve linked to the selected record or someone else has linked a chat with you as a participant. 
- Suggested contacts: Lists suggested contacts depending on the users who are working on the record. For more information, see [Use suggested contacts to collaborate with the right coworkers](teams-use-suggested-contacts.md).  
- Other chats/All recents: Lists your top 50 chat conversations on Teams. You can select any existing conversation and link it to a record. 

## Start a new linked chat

You can start a new linked chat or convert an existing Teams chat into a linked chat to associate the chat with a Dynamics 365 record. Standard record types, including case, conversation, account, contacts, knowledge article, and email, are available out-of-the-box, or your administrator can add your desired record type.

Your administrator can configure an optional message that you can send when using the chat to start a collaboration. This helps you to share succinct, read-only context with your collaborators on Teams.
 
If you're using Teams for the first time within Customer Service Hub or Customer Service workspace, you can select the blue bubble, and then follow the interface guidance.

1.	Open any Dynamics 365 Customer engagement record, and then select the **Teams chats and channels** integration icon.
    The **Teams chats (preview)** panel opens.
    - You can access the embedded chat from in Customer Service Hub and custom apps. When you select the Teams chat :::image type="icon" source="media/teams-icon.png" border="false"::: icon, the chat pane opens as an app in the right-side pane.
    - If you're in a multisession app, such as Customer Service workspace, you can access the chat pane directly from the productivity pane.
       > [!NOTE]
       > You can also access the chat pane from the home session in Customer Service workspace. When using the chat pane from the home session, you'll see two sections: Chats linked to other records and Other chats (if enabled by your administrator).
    
2.	Use one of the following methods:<br>
    a.	To start a new linked chat with a participant, select **New linked chat** in the **Linked to this record section** Type the name(s) of the participant(s) you want to chat with. You can start with just one collaborator and then progressively add more as needed (see step 6). Every new linked chat starts fresh, without bringing context from one-to-one chats or other chats you may have had with the participants. Therefore, it's important to name your chats appropriately to match the context of the record and conversation. For more information, see step 3. <br><br>
    b.	To start a linked chat with a suggested contact directly on the chat list, select the contact with whom you want to chat, and then select **Start a linked chat**.<br> 
    
     > [!div class="mx-imgBorder"] 
     > ![Start a linked chat.](media/teams-start-linked-chat.png "Start a linked chat")
     
     > [!NOTE]
     > You can only link group chats to records. Direct, one-to-one chats can't be linked, and will instead display an option to start a new linked chat with that contact.
       
3. The chat name uses the record name or the participants’ name, depending on the configuration that your administrator has set up. To set the chat name as the record name, you can ask your administrator to turn on the **Use record title as the default chat name for linked chats** setting. You can modify the chat name. Provide a meaningful name to the chat so that you can identify the chat even on Teams, and so that your collaborators on Teams can also easily identify chats that are associated with Dynamics 365 records.<br><br>
4. Your administrator can configure an optional message that you can send when using the chat to start a collaboration. The introduction message uses selected data fields from the associated record. This helps you to share succinct, read-only context with your collaborators on Teams. The message also includes a link to view the associated record in Dynamics 365. If your collaborators have a Dynamics 365 license and access to the record, they can view the full record details in a browser tab.
    
     > [!div class="mx-imgBorder"] 
     > ![Send an introduction message when using the chat.](media/teams-send-intro-message.png "Start a chat with an introductory message")
     
5. To convert an existing group chat into a linked chat, select a chat from the **All recents** section. Select the **More Commands** ellipsis (…), and then select **Link chats to record**. <br> 
    
6. (Optional) You can add more participants to the chat directly from the chat control by selecting the **View and add participants**.
    
     > [!div class="mx-imgBorder"] 
     > ![Add more participants to a chat.](media/teams-view-add-participants.png "View and add participants.")

        
## Link or unlink an existing chat from a record

You can link a chat to a single record or multiple records. For example, if you had a chat about a case that turned into a work order, you could also link the chat to the work order. If you decided later that you didn't want the chat linked to the case, you could unlink it if your administrator has given you the proper rights. For this example, you'd follow these steps:

- To link the chat to the case, select the chat, and then select **Link to this case**.
     
    > [!div class="mx-imgBorder"] 
    > ![Link an existing chat to a record, such as a case.](media/teams-link-chat.png "Link existing chat to a record")

- To unlink the chat from the case, select the chat, and then select **Unlink from this case**.

    > [!div class="mx-imgBorder"] 
    > ![Unlink an existing chat from a record, such as a case.](media/teams-unlink-chat.png "Unink existing chat from a record")
    
### Understand how unlink chat rights are assigned

As an agent, you have the following three options for getting rights to unlink chats, all of which are controlled by your administrator.

- You are the record owner, and your administrator enables this capability.
- You are the most recent user to link the chat to the record, and your administratior enables this capability.
- Your administrator assigns the right to unlink chats to you if you need the ability to unlink chats from records.

If your administrator hasn't assigned any of the above rights to you or your role, you won't be able to unlink any chat that you or other users have linked to records. If you need the ability to unlink chats from records, ask your administrator to set assign the rights to you.

## Use suggested contacts

The suggested contacts list displays users who are connected or have interacted with the record. Suggested contacts might include a team admin or members who've logged an activity in the record timeline, and so forth. There are two different types of suggestions: AI-based and rules-based. For more information, see [Use suggested contacts to collaborate with the right coworkers](/dynamics365/customer-service/teams-use-suggested-contacts).

## Link a Teams channel to a record

The **Channels** tab lists the channels that either you’ve linked to the selected record or someone else has linked a channel where you’re a participant. If you've linked a record to a channel using basic or enhanced collaboration experience, that channel is also listed in this tab. 

You can link relevant Teams channels to a record so that all the members can easily access the linked channels from the record and follow the conversation. 

1.	Open any Dynamics 365 Customer Service record, and select the Teams chat :::image type="icon" source="media/teams-icon.png" border="false"::: icon.<br>
   The **Teams chats (preview)** pane opens.
2. Select the **Channel** tab. The tab lists the channels that are already linked to a record.
3. Select the **Link channel** icon in the upper-right corner of the Teams chats (preview) pane.<br>
   The **Collaborate with Microsoft Teams** dialog opens.
4. To start a new linked channel, select **Create a new connection**.
5. To link an existing channel, select the channel from the list, and then select **Start collaboration**.

## Join a chat

As an agent, you can view and easily join chats that are linked to a record you have write access to, even if you weren’t originally a participant in the chat. Some scenarios where this can be useful include:

- **Case transfers**: If you’ve onboarded to a case that was previously handled by another agent, you can join the chat to better understand the context of the case, and then continue to collaborate with your relevant colleagues.
- **Case escalations**: If a case needs attention from someone with specific knowledge, the subject-matter expert who reviews it can participate in the relevant conversations.

 > [!NOTE]
 > You can only join linked chats, and to do so, you must have write access to the record and your admin has turned on the Join Chat capability for the record type in which you want to join any existing linked chat.

**To join a linked chat**:

1. Open the record for which you want to join the chat.
2. In the **Teams chats (Preview)** page, go to any of the linked chats you want to join. A lock icon is displayed with text that says "Hover over to join this chat". When you hover over the lock icon, if have write access to the associated record, a **Join** button will be displayed.

    > [!div class="mx-imgBorder"] 
    > ![Text that says to hover over it to join the chat.](media/hover-join-chat.png "Display of text that says to hover over it to join a chat")

  > [!NOTE]
  > If you don't see the text that allows you to hover and join a chat, there are three possible causes for this:<br> 1) Your administrator hasn’t enabled Join chat capability for the entity.<br> 2) You have read-only access to the record.<br> 3) Both scenarios in 1 and 2 apply.<br> In any of these scenarios, you can ask a member of the chat to manually add you, or you can ask your administrator to turn on the Join chat capabilities for that record type. 

3. Select **Join**.<br>

    > [!div class="mx-imgBorder"] 
    > ![Join button for joining a chat.](media/teams-join-chat.png "Join button for joining a chat")

   The Teams popup chat will show that you’ve been added to the chat, and you'll have access to the entire chat history. Other chat members will also receive the system message that you've been added to the chat.
 
  > [!NOTE]
  > When a user is added using Join chat, any users who are chatting directly from Dynamics 365 apps will see a system message that says an unknown user added the new user to the chat and shared all of the chat history. This is a known issue that is specific to the embedded chat experience, and we are working to resolve it.<br>
  
   > [!div class="mx-imgBorder"] 
   > ![Text that says unknown user was added to a chat.](media/unknown-user-error.png "Display of text that says to an unknown user was added to a chat")

If you are using the Microsoft Teams app, when joining a chat, the following message is displayed: Dynamics 365 collaboration with Microsoft Teams added &lt;user name&gt; to the chat and shared all chat history.

   > [!div class="mx-imgBorder"] 
   > ![Text that says a user was added to a chat.](media/teams-chat-user-added.png "Text that says Dynamics 365 collaboration with Microsoft Teams added a user to a chat")
    


### See also

[Configure Teams chat in Customer Service](configure-teams-chat.md)<br>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
