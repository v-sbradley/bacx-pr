---
title: "Deleting or renaming topic files | MicrosoftDocs"
ms.date: 08/30/2018
ms.service: 
ms.topic: "conceptual"
author: "buck1ey"
ms.author: "buckg"
manager: "renwe"
---

# Deleting or renaming topic files

Deleting or renaming a topic file in GitHub will cause any existing links to the topic to error on docs.microsoft.com. To give customers a better experience, we can put redirections in place.

There are also localization considerations with deletions and renames. If the deleting or renaming isn't coordinated correctly, the localization handback can fail.

> [!NOTE]
> We have introduced a new validation check in GitHub for deleted/renamed files for Pull-Requests targeting master branch. This validation check will run along with other build checks by OPS when a pull-request is created. Once the check is finished validating, it reports back the deleted files (if any) as a comment in the pull-request similar to build comments. If any deleted files are reported by the new validation check for pull-request, please add back the deleted files and follow the listed steps to mitigate the pull-request build error for deleted/renamed files.
> Currently the validation check is enabled only for the **Customer-Engagement** repository.

Follow this process for deleting or renaming a file.

 1.  Writer/Editor updates TOC, planned features, change history, and any other topics referencing the removed content. They then coordinate the appropriate reviews and push the changes to "master."
These changes can be pushed live at any time. They will effectively hide the removed content from users. Actually deleting/renaming the topic needs to be timed with localization.

 1.	Writer/Editor opens TFS item, using [this template](https://dynamicscrm.visualstudio.com/OneCRM/_workitems/create/Task?templateId=adfeaa5a-22a9-4416-9755-9b9980c42822&ownerId=74778d57-e6a1-43fe-b56b-be19cb488aae), for CE listing topics to delete, and redirection target for each deleted topic. *If you don't have access to the OneCRM TFS instance, go to [http://myaccess](http://myaccess) and request access to either **CRM FTE Dev/Test Source Read-Write** (for FTEs), or **CRM Vendor Source** (for vendors).*
 
 1.	CE coordinates timing with localization
 
 1.	CE deletes topic(s), and implements redirect(s) in a working branch
 
 1.	CE opens PR from working branch to "master", adds Writer/Editor as reviewer
 
 1.	When approved by Writer/Editor, CE merges to "master" and deletes working branch


