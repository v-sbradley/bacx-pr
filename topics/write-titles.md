---
title: 'SEO: Tips for writing titles - Contributor Guide'
description: This article helps you write titles that fit the search result and scan better, by using examples from published documentation. The titles follow guidance from SEO basics, a useful guide to basic SEO techniques. 
author: ReneeW-CPub
ms.author: renwe
ms.date: 11/07/2019
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: internal-contributor-guide
---

# SEO: Tips for writing titles

This article helps you write better titles, by using examples from published documentation. The titles follow guidance from [SEO basics](https://review.docs.microsoft.com/help/contribute/contribute-how-to-write-seo-basics?branch=master), a useful guide to basic SEO techniques.
  
The title tag is important for SEO and visitors. The title string displays as the content title in the SERP (search engine result page) and in browser tabs. It's the most important factor in search ranking of the article. Its primary job is to tell visitors and search engines what they can expect from the web page in the most concise way possible.

> [!IMPORTANT]
> Don't confuse title with H1; they are two different text elements. The H1 displays at the top of the doc page and has a limit of 100 characters including spaces. The title tag is in article metadata and displays in the browser bar and on the search engine result page.

## Rules for writing titles

- **Preview the title text for clear intent.**  Paste the title into [Moz title tag preview](https://moz.com/learn/seo/title-tag). 
    - Is there enough information to understand what the article is about? 
    - Are key, differentiating terms and keywords at the head of the title?
- **Optimal: Maximum 60-65 chars including spaces and brand (titleSuffix), but *preview* your title.** Don't sacrifice clarity or service/product brand to fit. 
- **Product brand is required.** Brand can truncate in the search result as long as the article intent is clear. For Azure services, make sure the service brand is in the title. It can be appended using spaces and a hyphen character:

     
```console
Description of article content - Product Brand
```


- Words that truncate in search results still help with search rank, but don't help users determine relevance.
    
- titleSuffix metadata can be used to enter brand on each article and at folder level and globally in docfx.json file.

## Check your title and description at author time in VS Code

The [Docs Authoring Pack for VS Code](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack) now includes a Search Results Preview to help verify that your title and description will be helpful for users when returned in search. Using publicly available information from Google, Search Results Preview generates an approximation of what your article title and description will look like when returned in Google search on Chrome with default font settings. This is the most common way people find content on Docs, accounting for more than half of all page hits. Because much of Google's algorithm is secret, the preview might not match exactly. But it gives you an idea of how your title will be truncated and what description users will see when they find your article via search. Use it to make sure you're providing the most helpful, relevant information.

To use Search Results Preview:

1. In VS Code with the Docs Authoring Pack, click `Alt+M` to access the Docs Markdown menu or `F1` to access the command palette.
1. Select `Search Results Preview` from the Docs Markdown menu or filter the command palette  to find `Docs: Search Results Preview`.
1. Preview will open in a side-by-side window.

Here's search preview for the current article:

:::image type="content" source="media/seo-basics/search-preview.png" alt-text="Screenshot of search preview in VS Code, showing the description and how the title is truncated." loc-scope="vs-code":::

## Meta title examples

**Example 1**: [https://docs.microsoft.com/azure/virtual-machines/linux/tutorial-manage-vm](https://docs.microsoft.com/azure/virtual-machines/linux/tutorial-manage-vm)

**Current title tag**: Tutorial - Create and manage Linux VMs with the Azure CLI (57 characters)

**Edited title tag** : Tutorial: Create & manage Linux VMs with Azure CLI (50 characters)

> [!TIP]
> To reduce title tag length, try removing connecting words and articles like “and” and “the”. A great way to replace “and” is with an ampersand “&”, and often “the” can be omitted without hurting the meaning of the title tag. For tutorials, you use "Tutorial" in the title to call attention to them and help them rank in search. 

**Example 2**: [https://docs.microsoft.com/azure/security-center/security-center-alerts-data-services](https://docs.microsoft.com/azure/security-center/security-center-alerts-data-services)

**Current title tag**: Threat detection for data services in Azure Security Center (59 characters)

**Edited title tag**: Data services threat detection – Azure Security Center (54 characters)

> [!TIP]
> This example highlights the value of rearranging a phrase in order to reduce character length. In this case, switching the order of “Threat detection for data services” to “Data services threat detection” eliminated the need for the word “for” and saved some characters. Replacing “in” with a dash also minimized the length by a couple of characters. 

**Example 3**: [https://docs.microsoft.com/azure/security-center/security-center-just-in-time](https://docs.microsoft.com/azure/security-center/security-center-just-in-time)

**Current title tag**: Just-in-time virtual machine access in Azure Security Center (60 characters)

**Edited title tag**: Just-in-time VM access – Azure Security Center (46 characters)

> [!TIP]
> Another great way to shorten title tags is by replacing industry terms with common acronyms, when they are widely known and adopted. In this example, using the acronym for “virtual machine”, “VM”, shortened the title tag by quite a bit. Replacing “in” with a dash also reduced the length by a couple of characters. The meaning of the title tag remains the same, but it is now shorter.

**Example 4**: [https://docs.microsoft.com/sql/relational-databases/logs/troubleshoot-a-full-transaction-log-sql-server-error-9002?view=sql-server-2017](https://docs.microsoft.com/sql/relational-databases/logs/troubleshoot-a-full-transaction-log-sql-server-error-9002?view=sql-server-2017)

**Current title tag**: Troubleshoot a Full Transaction Log (SQL Server Error 9002) - SQL Server (72 characters)

**Edited title tag**: Error 9002: Troubleshoot transaction log – SQL Server (53 characters)

> [!TIP]
> With this example, the title tag was shortened by removing some repetitive phrasing (SQL Server mentioned a second time). The error code was moved to the head of the title, because keyword research shows users often search on them. A few optional words (“full”, “a”) were also removed to reduce the overall length. The SQL Server brand is programmatically appended in both versions.

**Example 5**:  [https://docs.microsoft.com/learn/modules/build-ml-model-with-azure-stream-analytics/](https://docs.microsoft.com/learn/modules/build-ml-model-with-azure-stream-analytics/)

**Current title tag**: Analyze images in real time with machine learning, Azure IoT Hub, and Azure Stream Analytics - Learn (100 characters)

**Edited title tag:**: Analyze images with machine learning, Azure IoT hub, & Stream Analytics - Learn (79 characters)
> [!TIP]
> In this example shortened the length by removing the extra words and keeping all the keywords intact including the brand.

**Example 6**: [https://docs.microsoft.com/aspnet/core/host-and-deploy/azure-iis-errors-reference?view=aspnetcore-2.2](https://docs.microsoft.com/aspnet/core/host-and-deploy/azure-iis-errors-reference?view=aspnetcore-2.2)

**Current title tag**: Common errors reference for Azure App Service and IIS with ASP.NET Core (71 characters)

**Edited title tag**: Common errors - Azure App Service & IIS with ASP.NET Core (57 characters).
> [!TIP]
> With this example, a very specific title tag was shortened by removing some optional words and adding a dash. These tweaks tightened the wording of the title tag so the entire title intent is readable on the search page.

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
