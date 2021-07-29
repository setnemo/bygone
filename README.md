# Bygone project

Save your old buggy code as a souvenir (git history included)


## How it work?

- fork this project
- open Settings > Secrets
- create 5 secrets
  - ARCHIVED_REPOSITORY - please add username/projectName for saving to arhive repo
  - ARCHIVE_REPOSITORY - real arhive repo, format username/projectName
  - ARCHIVE_REPOSITORY_DEFAULT_BRANCH - main or master
  - GIT_USERNAME - your username at Github for pushing to arhive repo
  - WRITE_GITHUB_TOKEN - your github api token with write rules for pushing to arhive repo
- open Actions > archivist and press 'Run workflow'
- enjoy!

Example arhive repo: [setnemo/arhive](https://github.com/setnemo/archive/tree/main/setnemo)

## What will be added to the archive?

Bygone create new folder like username/projectName/branchName and save all branches with git history.

## How can I archive more than one project?

Just update ARCHIVED_REPOSITORY to another repo and run workflow again

----
> MIT License, Artem Pakhomov, 2021
