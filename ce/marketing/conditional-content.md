---
title: "Preview: How to use conditional content (Dynamics 365 Marketing) | Microsoft Docs"
description: "Learn how to use conditional content features in Dynamics 365 Marketing."
ms.date: 06/01/2022
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

# Preview: How to use conditional content

> [!IMPORTANT]
> A preview feature is a feature that is not complete, but is made available before it’s officially in a release so customers can get early access and provide feedback. Preview features aren’t meant for production use and may have limited or restricted functionality.
> 
> Microsoft doesn't provide support for this preview feature. Microsoft Dynamics 365 Technical Support won’t be able to help you with issues or questions. Preview features aren’t meant for production use, especially to process personal data or other data that are subject to legal or regulatory compliance requirements.

## How to enable the conditional content preview

This article refers to a feature that is in preview and may not be enabled in your environment. If you don’t see this feature in your app, contact your admin who can activate it by going to **Settings** > **Other settings** > **Feature switches** > **Personalization** and enabling the **Conditional content in email editor** feature switch.

> [!div class="mx-imgBorder"]
> ![Screenshot of the conditional content feature switch.](media/conditional-content-switch.png "Screenshot of the conditional content feature switch")

## What is conditional content?

Conditional content is an easy way to deliver effective and engaging personalized content. A simple example of conditional content is including different images based on a recipient’s profession, age group, address, interests, or other such factors. Creating this kind of personalized content in Dynamics 365 Marketing is straightforward, requiring no coding or scripting. Here is a short video that shows conditional content in action:

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4Yb7B]

Conditional content, as the name implies, consists of two parts: condition and content. The combination of these two parts is called a “variation.” You can create as many variations as needed. At the time an email is sent, conditions are evaluated in the order they're present in the email. When a condition is satisfied, the corresponding content is included and the conditional evaluation stops. If none of the conditions are satisfied, the default content is used. If there's no default content, then no content is included.

Conditional content can be a section or an image:

- A conditional section can include text, images, buttons, links, or any other element that is supported by the email editor.
- A conditional image only includes images.
- A conditional section can't include a conditional image.

> [!NOTE]
> A conditional image must have default content whereas default content is optional for a conditional section. This prevents delivering emails with misaligned layouts.

## When should you use conditional content?

Conditional content is a great way to personalize email content. Here are some ways you can use conditional content:

1. Include different images that match the recipient’s interests (for example, sports or hobbies).
1. Deliver different content based on the recipient’s demographic information (for example, city or state of residence, gender, or age).
1. Use different language content using the recipient’s preferred language or region/country.
1. A common usage is within footer where you may need to change some content (for example, social links or legal text) depending on the recipient’s information.

## Working with conditional content

This section explains how to create, delete, preview, and test conditional content.

### Create

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4Yb7A]

1. In the email designer, select a section (or an image) and then select the conditional content button.

    > [!div class="mx-imgBorder"]
    > ![Screenshot of the conditional content button.](media/conditional-content-button.png "Screenshot of the conditional content button")

1. The section (or the image) frame changes color to indicate it's now a conditional section. The property pane on the right margin shows a new sub-tab called **Variation**. Select the **Variation** sub-tab.
1. Select **+ New Condition** in the property pane. Define the condition.
1. Add more conditions if needed. At this point, you have the same content associated with each condition.
1. Select **Default** on any condition for which you want to change the content.
1. Update the section (or image) in the designer.
1. Repeat the previous two steps to update all the content as needed.

### Delete

1. In the email designer, select a conditional section (or a conditional image) and then select the conditional content button
1. This will convert the conditional section (or the conditional image) into a normal section (or image) by deleting all conditions and associated content. The default content (or the first condition’s content if there's no default) is retained in the designer.

### Preview and test

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4YmOM]

In the designer, you should always preview and test each variation to make sure there are no unexpected results. To preview and test, follow the steps below.

1. Select the **Preview and test** tab in the email designer and then select **Edit sample data**.
1. In the property pane, expand the **Conditional content** section.
1. **Email variation** lists all possible variations of the email. Select the variation you want to check. The main designer area will show the preview of that variation.
1. By default, variations are named using the names you gave to the conditions. If desired, you can rename the variation by updating its name in **Variation name** edit box.