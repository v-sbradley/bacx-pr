---
title: "Feature: Holdback plans"
ms.date: 09/01/2020
ms.service: 
ms.topic: "conceptual"
author: "emceachern"
ms.author: "emcheachern"
manager: "renwe"
---

# Feature: Holdback plans

**Persona:** Product Marketing Group (PMG) & Content Publishing Team

**Why this feature:**

The Product Marketing team did not have the ability to hold back a release plan within the release planner app. PMs were asked to set “Include in Release Plan” to No to stop features from publishing which introduced risk. If someone accidentally sets the “Include in Release Plan” to Yes, the plan could potentially be published in the next publishing cycle. In order to help this situation, we have introduced a holdback feature which appears as an editable field in the marketer’s form and as read-only in the contributor’s form.

**How does it work:**
-	This feature allows the PMM to associate a release plan to a marketing or newsworthy moment. 
-	Once the feature is set as holdback, it will not be pushed into GitHub to continue the publishing cycle until at least after the disclosure date of the marketing moment has passed.


