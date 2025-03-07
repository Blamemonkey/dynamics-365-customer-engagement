---
title: "Known issues in real-time marketing (Dynamics 365 Marketing) | Microsoft Docs"
description: "Learn about known issues in real-time marketing and how to work around them."
ms.date: 06/02/2022
ms.custom: 
  - dyn365-marketing
ms.topic: article
author: alfergus
ms.author: alfergus
manager: shellyha
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365Mktg
---

# Known issues in real-time marketing

As we continue to work on real-time marketing and refine the experience, we've become aware of some outstanding issues for you to bear in mind. These issues are summarized in this article.

## Analytics

- In the aggregate cross-journey analytics dashboard, an extra step is needed to load the Power BI report in the Android and iPad native apps. To load the report, go to **Analytics**, then select a row, select the **Show as from** sub menu, then select **CC_Analytics_ReportingControl**.
- Data retention is 12 months for details of operational data (such as contacts impacted by delivery and interaction issues) and for all other metrics (including operational and aggregate analytics).
- Some strings in the Power BI aggregate analytics dashboard aren’t localized.

## Consent

- Only one email address can be checked for consent for contacts.
- Only one physical address field is available for commercial emails.

## Customer journeys and orchestration

- The journey goal only counts unique profiles. Unique profiles are the number of unduplicated (counted only once) people that enter the journey. This means that in cases where the journey is a repeating journey, the total inflow won’t match the number of unique profiles with which the goal attainment is calculated.
- The journey goal met in analytics currently counts the number of unique profiles that met the goal divided by the total inflow. This will be fixed soon to count unique profiles that met the goal divided by total unique profiles.
- After a real-time marketing journey is migrated, restored, or copied, its state is changed from **Live** to **Stopped**. To restart a migrated, restored, or copied journey, you need to first duplicate the journey, and then execute it.
- Customer journeys have a limitation of eight nested conditions.

## Dynamics 365 Customer Insights

-	Segments and profiles in Customer Insights aren’t evaluated in real time. Segments and profiles can be set to refresh on a schedule defined by the Customer Insights admin. When a customer journey uses profiles from Customer Insights, the earliest you can engage with a new customer is when their profile is created on the next scheduled refresh. Similarly, when you use segments from Customer Insights, new customers will only enter the journey on the next scheduled refresh.
-	Once you start using Customer Insights data in customer journeys, you can’t remove the profile attributes being used from the data unification process (Map-Match-Merge). Doing so might break customer journeys and personalization tokens that reference those attributes.
- Customer Insights segments used in customer journeys can’t currently exceed 10 million profiles. A larger sized segment may get truncated to the first 10 million profiles only.

## Email editor

- The real-time marketing email editor *doesn’t* contain the following capabilities from the outbound marketing email editor: video, content blocks, QR codes, Teams check-in links, marketing page links, or the Send now function.
- Emails created in outbound marketing need to be recreated in the real-time marketing email designer to be used in real-time marketing.
- Content blocks may not be editable immediately after inserting into an email. When a content block is added to an email, its content may not be editable (cannot be selected). To work around this issue, refresh the page.

## Triggers

- You can’t instrument C# apps in real-time marketing. If you choose to use an alternate language like Python, you’ll have to manage an infra to run Python.
- Published triggers can’t be migrated when moving data between environments. Any published triggers in the old environment need to be re-created in the new environment. Draft triggers, however, can be migrated as described in [Move custom triggers between environments](real-time-marketing-move-triggers.md).

## Natural language

-	Natural language for journey conditions isn’t compatible with events or behavioral attributes.
    - "Customers that opened an email" isn’t a phrase we currently support.
-	The entity type of the journey will follow the entity type the journey is bound to.
    - If the journey is contact-bound, the natural language will also require the term "contact."
    - If the journey is customer profile-bound, the natural language will also require the term "customer."

## Personalization

- Changing the data binding of existing dynamic text creates new dynamic text.
- Even if you delete all usage of a piece of dynamic text from the current message, it is still shown and considered in use.

## SMS

- Currently limited to one phone number.
- Only United States numbers are issued (even when using the app in the United Kingdom).
