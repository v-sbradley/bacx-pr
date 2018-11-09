# Permission Levels

[GitHub repos managed by crmce](crmce-repos.md) use three GitHub teams to manage permissions to GitHub repos. An additional two access levels don't require GitHub teams, resulting in these 5 levels.

|Level   | GitHub Team  |Notes   |
|---|---|---|
| Public  |n/a   | Anyone with a GitHub account has access to Microsoft _public_ repos. They can create forks, make content suggestions, and raise pull requests.  |
| MicrosoftDocs  |n/a  | Any member of the MicrosoftDocs GitHub organization has read access to Microsoft _private_ repos. This requires a corporate network account. They can create forks, make content suggestions, and raise pull requests.  |
| Contributors  | [bacx-contribute](https://github.com/orgs/MicrosoftDocs/teams/bacx-contribute/members)  | Anyone outside BACX team who contributes to the repos. They have write access, can create branches, and can raise pull requests. They can't push content to _master_ or _live_ branches on their own.  |
| BACX  | [bacx-write](https://github.com/orgs/MicrosoftDocs/teams/bacx-write/members)  | Everyone on the BACX team. They have write access, can create branches, and can push/merge content to the _master_ branch on their own (with one approved review).  |
| Admin | [bacx-admin](https://github.com/orgs/MicrosoftDocs/teams/bacx-admin/members)  | Leads, power users, and content engineering. They have full access to all repos and can push content to the _live_ branch. They are also _maintainers_ on all the BACX permission teams.   |
