---
title: "Explore the release plans repo"
ms.date: 10/29/2018
ms.service: 
ms.topic: "conceptual"
author: "ReneeW-CPub"
ms.author: "renwe"
---
# Explore the release plans repos


We are currently using three repos for release plans content:

[Dynamics 365](https://github.com/MicrosoftDocs/dynamics-365-mixed-reality-pr). For Dynamics 365 wave 2 (October '19) release plans and later.<br/>
[Power Platform](https://github.com/MicrosoftDocs/powerplatform-releasenotes-pr). For Power Platform wave 2 (October '19) release plans and later.<br/>
[BusinessApplication-ReleaseNotes](https://github.com/MicrosoftDocs/BusinessApplication-ReleaseNotes). For April '19 release notes and earlier.

The root of the release plans repos contains an **articles** folder, which has a version folder for each release wave (such as 2019wave2 or April19).

<!-- editors note: Add dates for preview features for wave 2. -->

- The 2019 release wave 2 is for features releasing between October 2019 and March 2020.
- April '19 release notes are for features releasing between April 2019 and September 2019 and for preview features going into preview between February and July 2019.  

Each version folder contains:
- **toc.md**, which controls the left nav for all products in that release.
- **change-history.md**, which contains information about additions, deletions, and other changes in all products in that release.
- A folder for each product area. 

Each product area folder contains:
- **index.md**: A topic that summarizes the product area.
- **planned-features.md**: A topic that indicates a release date for each feature.
- A topic for each feature.
