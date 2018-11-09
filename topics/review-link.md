# Review links

There are multiple methods for finding, or creating, review links for content in your branches.

## Finding reivew links

### OPS build email

Each time you commit a change, the build system ("OPS") generates a build. When that build completes (or fails), the OPS system sends a status email message. The subject line for these messages will be **[Succeeded With Warning] Open Publishing Build Service - Publish**, or similar. The text in the brackets can be "Succeeded", "Succeeded With Warning", or "Failed". These messages contain review links for pages that were successuflly built.

![Review links in build status email](media/review-email.png)

Click **View** to navigate to a review build of a particular page.

If you aren't receiving build status emails, check your GitHub notification settings.

  1. Navigate to [https://github.com/settings/notifications](https://github.com/settings/notifications). You may need to log in to GitHub.

  2. Under **Email notification perferences**, verify the email address in **Default notification email**, and make sure **Include your own updates** is checked.

Also check your Outlook rules to make sure the messages aren't beening blocked.

### OPS build portal

## Creating review links

### Hack an existing link

### Build one from scratch

> [!NOTE]
> It can be helpful to bookmark a review link or two for future reference.