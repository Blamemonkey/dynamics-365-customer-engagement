---
title: "Support multiple providers with Dynamics 365 Channel Integration Framework 2.0 | MicrosoftDocs"
description: "Use this topic to understand how you can support multiple providers in Omnichannel for Customer Service using Dynamics 365 Channel Integration Framework 2.0."
ms.date: 12/31/2018
ms.topic: reference
author: mh-jaya
ms.author: v-jmh
manager: shujoshi
ms.custom: 
  - "dyn365-a11y"
  - "dyn365-developer"
---

# Support for multiple providers

With Dynamics 365 Channel Integration Framework 2.0, organizations can configure multiple providers (first-party chat and third-party telephony providers) in the Omnichannel for Dynamics 365 Customer Service app. This enables agents to simultaneously work on multiple sessions catering to different customers on different channels (for example, first-party chat and third-party telephony providers), where each of these sessions belongs to a different provider. Agents can switch across these sessions as needed. Omnichannel for Customer Service brings one preprovisioned channel provider configuration. You can add other channel provider records and configure them. Here are the key features of this capability:

-   Sessions started using Dynamics 365 Channel Integration Framework 2.0 APIs are associated with the provider. Providers are notified about events on the session that only they have started.

-   Providers can open new tabs only in the sessions they have started.

-   Providers cannot programmatically switch sessions or close sessions. Agents can manually switch and close sessions.

-   If a provider session is not in focus, and there is a new event in that session (for example, a new unread message from a customer), you can use the ***requestFocusSession*** API to show the agent that the session not in focus requires attention.

> [!NOTE]
> As a best practice, it is recommended that sessions are started after taking agent consent using a toast notification.

> [!IMPORTANT]
> For information on how to integrate custom (in-house) messaging channel providers, see [Bring your own channel](../../bring-your-own-channel.md).

### See also

[What's new in Dynamics 365 Channel Integration Framework](../whats-new-channel-integration-framework.md)<br />
[Configure channel providers](../configure-channel-provider-channel-integration-framework.md)<br />
[Bring your own channel](../../bring-your-own-channel.md)


[!INCLUDE[footer-include](../../../includes/footer-banner.md)]
