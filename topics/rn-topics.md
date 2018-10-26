---
title: "Topic types and their requirements"
ms.date: 10/25/2018
ms.service: 
ms.topic: "conceptual"
author: "ReneeW-CPub"
ms.author: "renwe"
---

## Feature topics
- Don’t update any metadata tags except title and description.
- If you change a feature’s title, make the same change in these places:
  - the title tag of the topic for that feature 
  - the H1 of the same topic
    For features that will ship to public preview in the six-month window of the release, ensure that “(Public Preview)” appears at the end of the H1.
  -  the link from toc.md to the feature topic
  - the link from planned-features.md to the feature topic
  - the link (if any) from change-history to the feature topic
- Ensure that the description tag follows the same guidelines as other topics do for SEO, etc.
- Ensure that the body of the topic (everything after the H1) meets the same guidelines as other topics do: no PII, minimum resolution for screen shots is 1920, screen shots have the div class for borders, etc.


## Summary of what's new topics 

Feature column:
- Put the name of the feature. 
- When possible, make the name a link to the topic about the feature


Release type column:
- For features in public preview, use "Public Preview", not just "Preview". 


Cloud/Online or on-premises column:
-Use either "Cloud" or "Online" in the column heading, depending on which word your product uses. 
  - Cloud or on-premises
  - Online or on-premises


Date column:
- Use the month and year the feature is planned to ship. For example: April 2019


Weekly release column:
- Add date once we publish the first one


## Change history topic
If a change is made to a published topic, make sure it's represented in the Change history topic.

General guidelines:
- See the comments at the top of the change-history.md file for a template for each type of table you might need. Use those templates so we are consistent within the topic. 
Don’t create multiple entries for the same feature. For example, a feature may slip more than once, slip before being removed, etc. In those cases, just update the existing entry to the new date or move the entry to the table for removed features, etc. as appropriate.
- Do not put private preview features in the Release Notes.

Types of change tables:
- Feature section changed
- Feature added to Release Notes
- Release date changed
- Features removed

Feature column:
- Put the name of the feature. 
- When possible, make the name a link to the topic about the feature

Date column:
- Put the month and day 
- For features that are not scheduled, put "Undetermined"
- For features that are both not scheduled and might ship after the current release notes timeframe, put "Undetermined (may release after <month year>". For example: Undetermined (may release after March 2019)
  


## Overview topics
content here
