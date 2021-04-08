---
title: "Requirements for creating links"
ms.date: 5/11/2020
ms.service: 
ms.topic: "conceptual"
author: "ReneeW-CPub"
ms.author: "renwe"
manager: "renwe"
---

# Requirements for creating links

There are multiple ways to implement links to and from topics on docs.microsoft.com. When implementing a link to or from a topic, you need to be aware of how that link will be used, and how it functions, when deciding which method to use.

 - **Raw links** are original, fully qualified URLs, for example [https://www.microsoft.com](https://www.microsoft.com). This format should be used for links to other (non docs) sites when the link doesn't require locale information to render correctly.
 - **Relative links** are links from the docs.microsoft.com site to another topic on the docs.microsoft.com, for example [./index](./index). This is the only link format that will behave correctly within an air gapped cloud environment, and should be used whenever possible. See [Create relative links](#relative).
 - **FWLinks** use the *go.microsoft.com* redirection service, for example [https://go.microsoft.com/fwlink/?linkid=2158040](https://go.microsoft.com/fwlink/?linkid=2158040). This service allows localization to specify different targets for different locales. It should be used whenever the raw link includes a locale value and/or the target site does not render content based on the user's browser settings. This type of link will not work in an air gapped cloud environment. See [Create or use an existing FWlink](#fwlink).
 - **Aka.ms links** use the *aka.ms* redirection service, for example [https://aka.ms/BAGReleaseNotes](https://aka.ms/BAGReleaseNotes). This service does not provide localization support, but does allow custom URL values. It should only be used if the raw URL does not contain any locale information, and the target site redirects users based on their browser settings. This type of link will not work in an air gapped cloud environment. See [Create or use an existing aka.ms link](#aka).

**Use the following decision tree to determine the best format for linking.**

## Step 1

Will the link you are creating be embedded in a product or service?

| Yes | No |
|-----|----|
| Use the FWLink forwarding service for this link.<br/>See [Create or use an existing FWLink](#fwlink). | Go to [Step 2](#step-2). |

<a name="step-2"></a>

## Step 2

Are you linking from a topic on docs.microsoft.com to another topic on docs.microsoft.com?

| Yes | No |
|-----|----|
| Use a relative link.<br/>See [Create a relative link](#relative). | Go to [Step 3](#step-3). |

<a name="step-3"></a>

## Step 3

Does the link contain any locale information (i.e., "en-us")? If so, remove the locale and try to follow the link. Does it require the locale information to render correctly?

| Yes | No |
|-----|----|
| This URL will need to use the go.microsoft.com (FWLink) service.<br/>This allows the localization team to specify targets for each locale.<br/>See [Create or use an existing FWLink](#fwlink). | Go to [Step 4](#step-4). |

<a name="step-4"></a>

## Step 4

Is there a reason the link needs to use a link simplification and redirection service? Common reasons creating a shortened URL for social media, or a more memorable URL for marketing.

| Yes | No |
|-----|----|
| You can use the aka.ms service to simplify and redirect this link.<br/>See [Creating or using an existing aka.ms link](#aka). | Use the raw link in your content. |

<a name="relative"></a>

## Create relative links

Relative links are the best way to link between content on docs since they will function correctly in air-gapped environments, on the live docs site, and on the review site. The method of creating the relative path differs, depending on whether or not the target content is in the same repo and docset.

### Links to articles in the same docset

To link to an article in the same docset, use a *relative path* link. A relative path is the path to the target file relative to the current file. Use the following syntax to build a relative path:

- **file.md** or **./file.md** specifies a file that's in the same directory (folder) as the current file

- **ide/file.md** or **./ide/file.md** specifies a file that's in a child directory (subfolder) named **ide**

- **../file.md** specifies a file that's in the parent directory of the current directory

- **../../file.md** specifies a file that's two directories above the current directory

- **../ide/file.md** specifies a file that's in a directory named **ide** that's a peer directory of the current directory


For example:

```md
[link text](../../folder/filename.md)
```

Instead of constructing a relative path from the current file to the target file, you can start the file path at the root of the docset. This type of link starts with **~**. For example, if the docset's root folder is **docs**, the current file is **docs/ide/current-file.md**, and the target file is **docs/test/unit-test/load-tests.md**, the link is as follows:

```md
[load tests](~/test/unit-test/load-tests.md)
```

> [!TIP]
> Starting links with **~** produces invalid links when navigating source repositories on GitHub.

Include the **.md** file extension in all types of relative link. If you don't, the link may still work on the docs.microsoft.com site, but it won't work when you view the file on GitHub. Also, a build warning is generated at build time.

#### Advantages

Relative path links, that is, links that don't start with **/** and that do end with **.md**, are validated at build time. Build produces a helpful warning if there's a typo in the link, or if the file doesn't exist. For this reason, it's best to use a relative path for links to topics in the same docset. File-relative links are also click-navigable in the Visual Studio Code editor (however, root-relative links that start with **~** are not clickable in the editor).

### Links to articles in other repos or docsets

To create a site-relative link to an article in another docs repo or docset, use the part of the target URL that comes after the locale code. This makes the link functional on docs.microsoft.com, in air-gapped environments like JEDI, and in offline books (if that docset is published as an offline book). For example, to link to the article at **https://docs.microsoft.com/en-us/windows/uwp/get-started/get-set-up**, the link syntax is **/windows/uwp/get-started/get-set-up** as shown here:

```md
For more information, see [Get set up](/windows/uwp/get-started/get-set-up).
```

Don't append the file extension *.md* on a link to an article in another repo or docset.

Site-relative links aren't validated at build time like file-relative links. If you have a typo in your link, no warning is generated. 

<a name="fwlink"></a>

## Create or use an existing FWLink

  1. Go to [https://aka.ms](https://redirectiontool.trafficmanager.net/am/redirection/home?options=host:go.microsoft.com) and select "go.microsoft.com" in the **Host:** dropdown.

  2. Click **Advanced Filters**

  3. Add a filter for **Target URL** **Contains** and paste your target URL in as **Value**

  4. Click **Apply Filters**

  If the query returns results, select the copy icon next to the Link ID and use the copied URL.

  If the query doesn't return results, you'll need to create a new entry.

  1. Click **New Link**

  2. Fill out the appropriate information. Use **bacxfwlo** for **Security Group Alias** and your alias, and your manager's, for **Owner**.

  3. Click **Create**

  4. Once the link is created, click the copy icon next to the Link ID and use the copied URL.

<a name="aka"></a>

## Create or use an existing aka.ms link

  1. Go to [https://aka.ms](https://redirectiontool.trafficmanager.net/am/redirection/home?options=host:aka.ms) and select "aka.ms" in the **Host:** dropdown.

  2. Click **Advanced Filters**

  3. Add a filter for **Target URL** **Contains** and paste your target URL in as **Value**

  4. Click **Apply Filters**

  If the query returns results, select the copy icon next to the Link ID and use the copied URL.

  If the query doesn't return results, you'll need to create a new entry.

  1. Click **New Link**

  2. Fill out the appropriate information. Use **bacxfwlo** for **Security Group Alias** and your alias, and your manager's, for **Owner**.

  3. Click **Create**

  4. Once the link is created, click the copy icon next to the Link ID and use the copied URL.
