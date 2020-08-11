---
title: 'SEO: Tips for writing titles - Contributor Guide'
description: This article helps you write titles that fit the search result and scan better, by using examples from published documentation. The titles follow guidance from SEO basics, a useful guide to basic SEO techniques. 
author: ReneeW-CPub
ms.author: renwe
ms.date: 08/07/2020
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: internal-contributor-guide
---

# SEO: Tips for writing titles

This article helps you write better titles, by using examples from published documentation. The titles follow guidance from [SEO basics](https://review.docs.microsoft.com/help/contribute/contribute-how-to-write-seo-basics?branch=master), a useful guide to basic SEO techniques.
  
The title tag is important for SEO and visitors. The title string displays as the content title in the SERP (search engine result page) and in browser tabs. It's the most important factor in search ranking of the article. Its primary job is to tell visitors and search engines what they can expect from the web page in the most concise way possible.

> [!IMPORTANT]
> Don't confuse title with H1; they are two different text elements. The H1 displays at the top of the doc page and has a limit of 100 characters including spaces. The title is in article metadata and displays in the browser bar and on the search engine result page.

## Rules for writing titles

- Preview the title text for clear intent. Paste the title into [Moz title tag preview](https://moz.com/learn/seo/title-tag). 
    - Is there enough information to understand what the article is about? 
    - Are key, differentiating terms and keywords at the head of the title?
- Optimal: Maximum 60-65 chars including spaces and brand (titleSuffix), but *preview* your title.** Don't sacrifice clarity or service/product brand to fit. 
- Write titles using sentence case.
- Include specific information about the action or concept discussed in the article.  
- Avoid using product names in the title, unless you need to distinguish between different flavors of Dynamics 365.  
- Avoid using vague verbs, such as “Using” or “About.”  
- Avoid using gerunds, such as “Managing” or “Integrating.” 

## Check your title and description at author time in VS Code

The [Docs Authoring Pack for VS Code](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack) now includes a Search Results Preview to help verify that your title and description will be helpful for users when returned in search. Using publicly available information from Google, Search Results Preview generates an approximation of what your article title and description will look like when returned in Google search on Chrome with default font settings. This is the most common way people find content on Docs, accounting for more than half of all page hits. Because much of Google's algorithm is secret, the preview might not match exactly. But it gives you an idea of how your title will be truncated and what description users will see when they find your article via search. Use it to make sure you're providing the most helpful, relevant information.

To use Search Results Preview:

1. In VS Code with the Docs Authoring Pack, click `Alt+M` to access the Docs Markdown menu or `F1` to access the command palette.
1. Select `Search Results Preview` from the Docs Markdown menu or filter the command palette  to find `Docs: Search Results Preview`.
1. Preview will open in a side-by-side window.

Here's search preview for the current article:

:::image type="content" source="media/seo-basics/search-preview.png" alt-text="Screenshot of search preview in VS Code, showing the description and how the title is truncated." loc-scope="vs-code":::

## Meta title examples

**Example 1**

**Current title**: Understand how to prioritize your sales pipeline through the work list in Dynamics 365 Sales Insights  (101 characters)

**Edited title**: Prioritize your sales pipeline using a work list (50 characters)

> [!TIP]
> To reduce title length, try removing articles like “the”. Often “the” can be omitted without hurting the meaning of the title.  

**Example 2**

**Current title**: Frequently asked questions about synchronizing records between Microsoft Dynamics 365 apps and Microsoft Outlook  (113 characters)

**Edited title**: Synchronize records between Dynamics 365 apps and Microsoft Outlook FAQ (71 characters)

> [!TIP]
> This example highlights the value of rearranging a phrase in order to reduce character length. In this case, "FAQ" should always be used instead of writing out "frequently asked questions. Also, it's good to avoid using gerunds.

**Example 3**

**Current title**: Download Dynamics 365 Customer Engagement (on-premises) version 9.x Software Development Kit (SDK)  (98 characters)

**Edited title**: Dynamics 365 Customer Engagement (on-premises) version 9.x SDK  (72 characters)

> [!TIP]
> Another great way to shorten titles is by replacing industry terms with common acronyms, when they are widely known and adopted. In this example, using the acronym for “software development kit”, “SDK”, shortened the title by quite a bit. Removing "download" also reduced the length by a couple of characters. The meaning of the title remains the same, but it is now shorter.

**Example 4**

**Current title**: Use SideFX Houdini to prepare 3D models for use in Dynamics 365 mixed-reality apps (82 characters)

**Edited title**: SideFX Houdini - Prepare 3D models for Dynamics 365 mixed-reality apps  (70 characters)

> [!TIP]
> > With this example, removing some optional words like "use" and adding a dash made the title shorter. These tweaks also tightened the wording of the title so the entire title  is readable on the search page. A few optional words (“for use in”) were also removed to reduce the overall length. 

**Example 5**

**Current title**: Things to keep in mind before you start authoring in Dynamics 365 Guides  (82 characters)

**Edited title**: Get started authoring in Dynamics 365 Guides (Preview) (54 characters)

> [!TIP]
> In this example, you can shorten the length by removing the extra words and keeping all the keywords intact including the brand.

## How to add brand using titleSuffix metadata

Title suffix metadata allows you to enter brand using different methods.
As any other metadata topic level metadata overwrites folder level and global metadata.  Here are the examples for each type.

**Topic Level** You can add titleSuffix metadata on each article to append the title body with brand.

:::image type="content" source="media/seo-basics/titleSuffix-article.png" alt-text="brand-article":::

> [!IMPORTANT]
> Make sure titleSuffix metadata in entered with exact casing as "titleSuffix" with uppercase "S"

In the previous example, the full title in search becomes “Model training methods - Azure Machine Learning | Microsoft Docs”. The branding in titleSuffix contributes to the overall title length, so avoid repeating the full brand name in the title metadata. The advantage of this method is that all articles are consistently branded for search ranking.

**Folder Level (docfx.json)** Folder level metadata is entered in docfx.json file.  Here is an example from Azure-docs-pr repo

:::image type="content" source="media/seo-basics/titleSuffix-folder.png" alt-text="titlesuffix-folder":::


**Global metadata (docfx.json)** Brand (titleSuffix) can be set globally under Global metadata section of docfx.json file.
Here is an example from Xamarin repo

:::image type="content" source="media/seo-basics/titleSuffix-global.png" alt-text="titlesuffix-globally":::

> [!NOTE]
> For large repos with docs for many services and technologies, make sure you apply titleSuffix to the correct folder level titleSuffix.  Setting titleSuffix for an entire repo is useful only for repos containing docs for a product or service with a single brand. 
