---
title: "Best practices for creating links"
ms.date: 5/11/2020
ms.service: 
ms.topic: "conceptual"
author: "ReneeW-CPub"
ms.author: "renwe"
manager: "renwe"
---

# Best practices for creating links

Use the following decision tree to determine the best format for linking.

## Step 1

Are you linking from a topic on docs.microsoft.com to another topic on docs.microsoft.com?

:::row:::
   :::column:::
      **Yes**

      Use a relative link. Explanation of AGC. Link to [Creating relative links](#relative).
   :::column-end:::
   :::column:::
      **No**

      Proceed to [Step 2](#step-2)
   :::column-end:::
:::row-end:::

<a name="step-2"></a>

## Step 2

Does the link contain any locale information (i.e., "en-us")? If so, remove the locale and try to follow the link. Does it require the locale information to render correctly?

:::row:::
   :::column:::
      **Yes**

      This URL will need to use the go.microsoft.com (also known as FWLink) service. This allows the localization team to specify targets for each locale. See [Creating or using an existing FWLink](#fwlink).
   :::column-end:::
   :::column:::
      **No**

      Proceed to [Step 3](#step-3).
   :::column-end:::
:::row-end:::

<a name="step-3"></a>

## Step 3

Is there a reason the link needs to use a link simplification and redirection service? Common reasons include the need for a shortened URL for social media, or to create a more memorable URL for marketing.

:::row:::
   :::column:::
      **Yes**

      You can use the aka.ms service to simplify and redirect this link. See [Creating or using an existing aka.ms link](#fwlink).
   :::column-end:::
   :::column:::
      **No**

      Proceed to [Step 3](#step-3).
   :::column-end:::
:::row-end:::

<a name="relative"></a>

## Creating relative links

Information here about creating relative links on docs.

<a name="fwlink"></a>

## Creating or using an existing FWLink

  1. Navigate to [hhttps://redirectiontool.trafficmanager.net/am/redirection/home?options=host:go.microsoft.com](https://redirectiontool.trafficmanager.net/am/redirection/home?options=host:go.microsoft.com).

  2. Click **Advanced Filters**

  3. Add a filter for **Target URL** **Contains** and paste your target URL in as **Value**

  4. Click **Apply Filters**

  If the query returns results, select the copy icon next to the Link ID and use the copied URL.

  If the query doesn't return results, you'll need to create a new entry.

  1. Click **New Link**

  2. Fill out the appropriate information. Use **bacxfwlo** for **Security Group Alias**.

  3. Click **Create**

  4. Once the link is created, click the copy icon next to the Link ID and use the copied URL.

  


<a name="aka"></a>

## Creating or using an existing aka.ms link

  1. Navigate to [https://redirectiontool.trafficmanager.net/am/redirection/home?options=host:aka.ms](https://redirectiontool.trafficmanager.net/am/redirection/home?options=host:aka.ms).


