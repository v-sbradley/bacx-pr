---
title: "Explore the release plans repo"
ms.date: 08/21/2019
ms.service: 
ms.topic: "conceptual"
author: "ReneeW-CPub"
ms.author: "renwe"
---
# Explore the release plans repos

We currently use three repos for our release plans content:

- [dynamics365-releasenotes-pr](https://github.com/MicrosoftDocs/dynamics-365-mixed-reality-pr). For **Dynamics 365 wave 2** (October '19) release plans and later.

- [powerplatform-releasenotes-pr](https://github.com/MicrosoftDocs/powerplatform-releasenotes-pr). For **Power Platform wave 2** (October '19) release plans and later.

- [BusinessApplication-ReleaseNotes](https://github.com/MicrosoftDocs/BusinessApplication-ReleaseNotes). For **April '19** release notes and earlier.

Updated content is pushed from the Release Planner Tool to the two **wave 2** repos once a week, where it is edited, merged, and published. The team's editors manage this process.

For **April '19** content or earlier, doc owners make updates directly in the BusinessApplication-ReleaseNotes repo and create pull requests, which the team's editors manage.

No matter which repo is involved, the team's editors might reach out to doc owners via email if questions come up during the editing process. Typically, the editors enter questions or comments directly in the GitHub file using Markdown tags like this:

<!--editor: Please review the rewrite of the following sentence. -->

## Repo structure

The root of the release plans repos contains an **articles** folder, which has a version folder for each release wave (such as 2019wave2 or April19).

<!-- editors note: Add dates for preview features for wave 2. -->

- The **2019 release wave 2 plans** are for features releasing between October 2019 and March 2020.

- The **April '19 release notes** are for features releasing between April 2019 and September 2019 and for preview features going into preview between February and July 2019.  

Each version folder contains:
- **toc.md**, which controls the left nav for all products in that release.

- **change-history.md**, which contains information about additions, deletions, and other changes for all products in that release.

- A folder for each product area. 

Each product area folder contains:
- **index.md**: A topic that summarizes the product area.

- **planned-features.md**: A topic that includes a release date for each feature.

- A topic for each feature.
