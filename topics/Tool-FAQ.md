---
title: "FAQs for the Release Planner App| MicrosoftDocs"
ms.date: 11/13/2019
ms.service: 
ms.topic: "conceptual"
author: "emceachern"
ms.author: "emceachern"
manager: "renwe"
---

# FAQs for the Release Planner App

#### How do I move my feature from one release plan to another?
1. Click “Copy Release Plan” on the feature that you want to move.  
2. In the **copied release plan**, change the release wave to the corresponding release.   
**Note**: The feature name appears with a prefix “Copy - “ Don’t forget to update it. Also, tool will prompt you to select the public preview or a GA date within the wave before saving.  
3. On the existing plan (the plan you wanted to move from), toggle the Include in Release plan to No.  
4. Set one of the following values in the removal reason:
- Moved to the next release wave
- Moved to the previous release wave  
With this, the release plan will be moved from the current release and properly added to the corresponding release.
5. Make sure you toggle the “Include in release plan” to No and provide the reason in the removal reason drop down.   
 
#### How do I check to see what's changed in a feature entry?
In the entry, to go the "Related" tab. A short dropdown should appear, and select "Audit History" will will show you the history of the feature. 

#### What if I am still working on my feature and I don't want it to be released?
Make sure the toggle on the top of the feature is "No" for "Include in release plans."

#### If I update my detail, feature, or something else in the tool, when will it go live? 
The udpates will be included in the next publish which is shown on the schedule. 

#### Where do I find the schedule for the upcoming trains/publishes?
The [schedule](https://msit.powerbi.com/groups/fce55d85-50c2-4249-b054-60f8643ad13f/reports/0eb6f27b-2d3a-447d-9a6a-cf77f35bfbcd/ReportSection31aec9950d0006de8110) lives in the tool now. You can see what's included in the next publish, the dates, and what the upcoming dates look like. There are two tabs at the bottom of the schedule so you can toggle between waves. 

#### What do I do about the dates in the release plans if a feature is being released in different regions in a phased manner? 
Before a feature ships, use the month and year the feature is planned to ship. Example: April 2019
Once the features has shipped, use the day, month, and year. Example: April 12, 2019
If a feature is being released in different regions in a phased manner, use the date it first shipped regardless of the geo. For example, if a feature is released in Japan on April 11 and in North America on April 25, then use April 11, 2019 in the Date column. 

#### How do I create a view?
1. Find the "Create view" button at the top of the page.
2. Select it (make sure your pop-up blocker is turned off as this pops up in a seperate window).
3. Select the appropriate perameters, keeping in mind that you can pare down the results by choosing addtional fields (like Release Date, Owner, or Product). 
4. When you have all of your search perameters, hit "Results" under the exclamation point, and you will see the results of your view. 

Views can be saved, shared, and modified. Don't forget to pin your saved view if you use it often.

## Doc Writers

#### I only want my actionable item in the app. How do I get that?
You can create personal views. You can also share views with other writers.

#### As a doc reviewer, can I review other’s content and toggle “doc owner reviewed” to Yes?
No. The workflow will reset the field to no if you are not the assigned doc owner.

#### If I don’t review the content on time, what will happen?
If the plan was published earlier, the existing article will continue to be available publicly with no changes. If it is brand new topic, it won’t be published.

#### How do I ensure all the uploaded images are available in GitHub?
As soon as the image is uploaded, the image will be created in GitHub (master branch). 
When we create the PR as part of the sync, the PR will include that image. 
If the image is failed to upload, “Image created” value will be set to No. 
The daily digest email (sent to the leads) will also indicate this status. 

#### Can I delete and upload the image with the same name?
Deletion of an image in the tool will not delete in GitHub. The image is created in GitHub based on the image name uploaded in the tool excluding the special characters (- allowed) & noisy words. The image name in GitHub will always be in lowercase. So, uploading image with the same name will not be uploaded to GitHub.

If you want to replace the current image, you need to upload an image with the new name. If the image is referred within feature detail, the image name should be changed. If you wish to delete the old image, you can delete them in GitHub.

## Editors

#### I see some inconsistencies in Planned features or the topic that was not part of tool created PR. Can I update them in GitHub and expect the tool syncs them?
No. Planned features, change history, TOC are always created from the tool. Updating them in GitHub will not sync back. If you are updating an article (ms.topic: article), the following information will sync back.
- title (This will come back as Feature Name) (No special characters)
- description (This will come back as Summary) (No special characters)
- Business Value (content between <!-- bv start --> and <!-- bv end -->)
- Feature Detail (content between <!--feature detail start --> and <!--feature detail end -->)

If you are updating the overview (ms.topic: overview) or product area (L2) overview (ms.topic: structure) the following information will sync back
- The entire content in product overview between <!--overview start--> and <!--overview end-->
- The entire content in product area (L2) overview between <!--structure start--> and <!--structure end-->
- Description in product area (L2) (No special characters)   

If you are updating an article that was not part of the PR update, the changes will not sync back. Why? The delta sync will lock only the plans that are updated. If you are updating the content that was not locked by the tool, the reverse sync simply ignores the changes.

#### How do I change the Alt Text of an image?
The alt text should be updated in the tool. If the image is included within the feature detail, then it should be updated in the feature detail as well.

