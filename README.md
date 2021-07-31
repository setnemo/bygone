# [Bygone project](https://github.com/setnemo/bygone)

Save your old buggy code as a souvenir (git history included)

## How it work?

0. Create new repository for arhive your projects. 
1. Create a personal access token (not the default GitHub Actions token) using
   the instructions
   [here](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).
   Personal access token must have permissions: `read:user` and `repo`. Copy
   the access token when it is generated – if you lose it, you will have to
   regenerate the token.
2. [Fork](https://github.com/setnemo/bygone/fork) this project
3. If this is the README of your fork, click [this
   link](../../settings/secrets/actions) to go to the "Secrets" page.
   Otherwise, go to the "Settings" tab of the newly-created repository and go
   to the "Secrets" page (bottom left).
4. Create 5 secrets:
    - ARCHIVED_REPOSITORY - please add username/projectName for saving to arhive repo
    - ARCHIVE_REPOSITORY - real arhive repo, format username/projectName (from step 0.)
    - ARCHIVE_REPOSITORY_DEFAULT_BRANCH - main or master - default branch in archive repo
    - GIT_USERNAME - your username at Github for pushing to arhive repo
    - WRITE_GITHUB_TOKEN - your github api token from step 1.
5. Open [Actions > archivist](../../actions/workflows/main.yml) and press 'Run workflow'
6. Enjoy!
7. Star [this repo](https://github.com/setnemo/bygone) if you like it!

## Example archive

My arhive repo: [setnemo/arhive](https://github.com/setnemo/archive/tree/main/setnemo)

## What will be added to the archive?

Bygone create new folder like username/projectName/branchName and save all branches with git history.

## How can I archive more than one project?

Just update ARCHIVED_REPOSITORY to another repo and run workflow again

----
> MIT License, Artem Pakhomov, 2021
