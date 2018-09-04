---
title: "Deleting or Renaming Topics | MicrosoftDocs"
ms.date: 08/30/2018
ms.service: 
ms.topic: "conceptual"
author: "buck1ey"
ms.author: "buckg"
manager: "renwe"
---

# Deleting or Renaming Topics

Deleting or renaming a topic in GitHub will mean that any existing links to the topic will error on docs.microsoft.com. To give customers a better experience, we can put redirections in place.

There are also localization considerations with deletions and renames. If a file is out for localization when it is deleted, the localization handback with fail.

Here is the best practice for renaming or deleting a file.

 -  Writer/Editor updates TOC, planned features, and change history and pushes changes to "master"
   > [!NOTE]
   > These changes can be pushed live at any time. They will effectively hide the removed content from users. Actually deleting/renaming the topic needs to be timed with localization.
 -	Writer/Editor opens TFS item for CE listing topics to delete, and redirection target for each deleted topic
 -	CE coordinates timing with localization
 -	CE deletes topic(s), and implements redirect(s) in a working branch
 -	CE opens PR from working branch to "master", adds Writer/Editor as reviewer
 -	When approved by Writer/Editor, CE merges to "master" and deletes working branch


