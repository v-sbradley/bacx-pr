---
title: "Make major or long-running changes| MicrosoftDocs"
ms.date: 07/26/2018
ms.service: 
ms.topic: "conceptual"
author: "KumarVivek"
ms.author: "kvivek"
manager: "annbe"
---

# Make major or long-running changes

For a contributor who needs to make major changes or will be a frequent
contributor to a repository, he/she should **clone** the repo on his/her local
computer, and then make the updates in a branch. With this approach, you can
update files in a markdown editor of your choice instead of a browser. 

1. Ensure you have completed steps in [Get started](get-started.md).

2. Install [Git tools](https://gitforwindows.org/), accepting all the default
    values in the installation wizard.

2.  There are multiple ways to clone a repo to your local computer:
    - **Using cmdline**: To know more, see <https://help.github.com/articles/cloning-a-repository>
    - **Using GUI tool such as GitHub Desktop**: To know more, see <https://help.github.com/desktop/guides/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop>

        You can download **GitHub Desktop** tool here: <https://desktop.github.com/>  
        
    - **Within VS Code**: To know more, see <https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository>
    
    While cloning a repo, you will need the address (URL) of the repo. See
    [our repos](get-started.md#our-repos) section to find out the
    URL of the repo you want to clone.

3.  After cloning a repo to your local computer, create a branch to make your
    changes. [Visual Studio Code](https://code.visualstudio.com/) is the
    preferred tool to edit the .md files on your local computer.

    > [!TIP]
    > Install the [Docs Authoring Pack](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack) extension to help you as you edit files with features such as spell check, previewing includes files, and so on.

4. If you leave your branch open but don't update it for a few days, avoid merge conflicts by refreshing your branch with changes from the **master** branch before you make further updates.

    - To refresh your local branch in Visual Studio Code:
        1. Ensure that the name of your branch appears in the lower-left corner.
        1. Press Ctrl-Shift-G to open Source Control.
        1. Select the ellipsis > **Pull from** > **origin** > **origin/master**.
    - To refresh your local branch at a command prompt, type these commands:
        1. **git checkout** *BranchName*
        1. **git pull origin master**

5.  After making your changes, [create a pull
    request](https://help.github.com/articles/creating-a-pull-request/) from
    your branch to the **master** branch to merge your changes and publish live.

That's it! A writer will pick up your PR, merge it into the **master** branch, and publish your changes live. After merging your PR, the writer will delete your branch to avoid branch clutter in our repo.

> [!NOTE]
> Any **stale** branches (branches with no active pull requests and no activity for 8 weeks) will be deleted from our repo. If you have a special situation, please contact [crmce](mailto:crmce@microsoft.com).
