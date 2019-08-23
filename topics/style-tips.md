---
title: Style tips for release plans
ms.date: 08/21/2019
ms.service: 
ms.topic: article
author: almostdunh
ms.author: v-ladunh
ms.reviewer: renwe

---

# Style tips for release plans

Here are style tips to help you as you create and develop your release plan topics.

## Topic organization  

### Separate topics
To enable linking within a PDF, it’s better to have single-feature files than to group features together in a single file. 

### Heading levels
Don’t skip heading levels within a topic. The first level should always be a heading 1 (#) and the next lower-level heading should be a heading 2 (##). Don’t jump from a heading 1 to a heading 3 or lower.

### Feature names 

Feature names in planned features, the TOC, and change history should match the topic heading. This helps readers know they’ve landed on the right topic when they select the link to that topic. 

## Linking

### Other resources
When providing a link to another resource, use the resource title and add a hyperlink. Don’t use the URL alone as your link, and don’t use “here” as a link – let readers know what you want them to see. Example:

  For instructions on how to set up the duplicate detection job, see [Run system jobs to detect duplicates](https://docs.microsoft.com/Dynamics365/customer-engagement/admin/run-bulk-system-jobs-detect-duplicate-records).

### External links

**Important:** If you’re linking from a topic to a URL that is not part of the same release plans version, use the full URL. Otherwise, the link will break in the PDF. 
  
### URLs and localization 

Remove the language portion of a URL: **en-us/**  and then test the link to make sure it still works. Our users who read the release plans in other languages will appreciate not being directed to English topics. Also, if you put "en-us/" when it's not needed, localization vendors have to touch every link to place the correct language code. This adds to the cost of localization.

## Images

### No border tags
We don't use border tags with images ([!div class="mx-imgBorder"]) in release notes. When the release notes are converted to PDF, the tags result in a non-caption style and strip the alt-text from the PDF.

### Names in screenshots 

Check your images for names of people, companies, or other PII. Any names must be from Microsoft-approved fictitious names lists. More information: [Fictitious names](fictitious-names.md)

### Alt text 

In the image path, enter an informative description of the image within the straight brackets. This provides the **required** alt-text. It also will appear as a caption in the PDF.

Information entered within the quotation marks will appear online as hover text. 

Here is an example of both:

![Schedule assistant displays results on the hour as part of interval scheduling](media/filters-share.png “Schedule assistant displays results on the hour as part of interval scheduling”)


## Formatting and style

### Alerts (Note, Tip, Important, Caution, Warning)

Alerts are a Markdown extension to create block quotes that render on docs.microsoft.com with colors and icons that indicate the significance of the content. The following alert types are supported:

```markdown
> [!NOTE]
> Information the user should notice even if skimming.

> [!TIP]
> Optional information to help a user be more successful.

> [!IMPORTANT]
> Essential information required for user success.

> [!CAUTION]
> Negative potential consequences of an action.

> [!WARNING]
> Dangerous certain consequences of an action.
```

### Term-definition lists 

Use bold for the key word or term, followed by a non-bold colon. Example: 

  The features include:
  - **Queues**: A redesigned experience helps to prioritize and monitor the progress of the assigned work.
  - **Subjects**: A powerful mechanism to classify cases, knowledge base articles, products, and sales literature.
  - **Case settings**: Links cases together, enabling better response and tracking for common issues.

### Months 

Use the full name of the month in date columns of tables for planned features or change history. No need to abbreviate. 

### When writing, keep in mind

- The use of “we” (Microsoft) and “you” is OK, but don’t use “I” unless you’re writing a blog.
- Use exclamation marks sparingly, if ever.  



