---
title: "Topic types and their requirements"
ms.date: 10/29/2018
ms.service: 
ms.topic: "conceptual"
author: "ReneeW-CPub"
ms.author: "renwe"
---
# Topic types and their requirements
Here are general requirements for each type of topic we have in the Release Notes. 

Also check out these great examples of each type: 

- Feature: [Late Payment Prediction extension](https://docs.microsoft.com/en-us/business-applications-release-notes/October18/dynamics365-business-central/late-payment-prediction)

- Summary of what's new: 
  - Online-only table: [Summary of what's new for Dynamics 365 Omni-channel Engagement Hub](https://docs.microsoft.com/en-us/business-applications-release-notes/October18/service/customer-service-omni-channel-release-notes/planned-features)
  - Cloud/online or on-premises table: [Summary of what's new in Finance and Operations](https://docs.microsoft.com/en-us/business-applications-release-notes/October18/dynamics365-finance-operations/planned-features)

- Change history: [Change history](https://docs.microsoft.com/en-us/business-applications-release-notes/October18/change-history)
For example, see how Talent and PowerApps did their change history tables. 

- Overview: [Overview of Dynamics 365 for Finance and Operations October '18 release](https://docs.microsoft.com/en-us/business-applications-release-notes/October18/dynamics365-finance-operations/)



## Feature topics

- Start by saying the value proposition of the feature.
- Include screenshots or an image to help users see the benefits, if a visual element can add interest.
- Be as descriptive as you can. And go back when you know more to add more info. It's the number one piece of feedback we get from customers about the Release Notes. They want more details about your features. 
- Once a feature ships, make sure to add the links to the shipped docs that went with it so users can get as much info as possible.
- If you change a feature’s title, make the same change in these places:
  - the title tag of the topic for that feature 
  - the H1 of the same topic
  - For features that will ship to public preview in the six-month window of the release, ensure that “(Public Preview)” appears at the end of the H1.
  -  the link from toc.md to the feature topic
  - the link from planned-features.md to the feature topic
  - the link (if any) from change-history to the feature topic
- Ensure that the description tag follows the same guidelines as other topics do for SEO, etc.
- Ensure that the body of the topic (everything after the H1) meets the same guidelines as other topics do: no PII, minimum resolution for screen shots is 1920, screen shots have the div class for borders, etc.

If you are using the Flow/PA authoring tool, these are additional guidelines for you:
- Don’t update any metadata tags except title and description.

## Summary of what's new topics 

Feature column:
- Put the name of the feature
- When possible, make the name a link to the topic about the feature

Release type column:
- For features in public preview, use "Public Preview", not just "Preview". (We do not put private preview features in the Release Notes.)

Cloud/Online or on-premises column:
-Use either "Cloud" or "Online" in the column heading, depending on which word your product uses. 
  - Cloud or on-premises
  - Online or on-premises
 -Values for the cells can be "Cloud," "Online", "On-premises", or "Both". Only use "Both" if online and on-premises are shipping at the same time.

Date column:
- For before a feature ships, use the month and year the feature is planned to ship. Example: April 2019
- For once the features has shipped, use the day, month, and year. Example: April 12, 2019

Weekly release column:
- Use the same version information that customers are being given and make it a link to the corresponding weekly release notes topic.
- Please note this applies only to some teams, such as Flow.


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
- Put the name of the feature
- When possible, make the name a link to the topic about the feature

Date column:
- Put the month and day 
- For features that are not scheduled, put "Undetermined"
- For features that are both not scheduled and might ship after the current release notes timeframe, put "Undetermined (may release after <month year>". For example: Undetermined (may release after March 2019)
  

## Overview topics
It's important to write a strong overview that outlines all the investments for the product area you are covering, and to group those investments by themes. More guidance coming soon...
