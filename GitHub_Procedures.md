# GitHub and GitLab Procedures

How to use different features of GitHub and GitLab.

## Get Access to UGA Libraries GitHub

To be added as a member of the UGA Libraries institutional GitHub account:

1. [Set up an individual GitHub account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account) 
2. Email your GitHub name to the Head of Digital Stewardship
3. Accept the invitation sent to the email address associated with your GitHub account

## Archive/Delete a Repository 

If you are no longer using or maintaining code, you may want to archive or delete it. 
In most cases, archive the repository so we have a record of the past project. 
This will make the repository read-only and it will be clear that it is no longer being maintained. 

You might delete a repository if: 

- There are security risks with keeping the repository publicly available. These risks could include: 
  - Sensitive code like internal URLs, usernames, passwords 
  - Packages prone to security risks (requests, lxml, others) 
- The repository is minimal, meaning there isn’t much code or involved processes. 
- The code lives somewhere else that is being updated/monitored.

### How to Archive a Repository 

Archiving a repository will make it read-only.
Prior to archiving, update the README with the status of the project and why it was archived.

- [GitHub Instructions for Archiving a Repo](https://docs.github.com/en/repositories/archiving-a-github-repository/archiving-repositories)  
- [GitLab Instructions for Archiving a Repo](https://docs.gitlab.com/ee/user/project/settings/#archive-a-project) 

### How to Delete a Repository 

Deleting a repository will remove all code, processes, and content from a project. 

- [GitHub Instructions for Deleting a Repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/deleting-a-repository) 
- [GitLab Instructions for Deleting a Repo](https://docs.gitlab.com/ee/user/project/settings/#delete-a-project)

## Setting Up Dependabot

Dependabot is a GitHub feature that automatically checks your packages/libraries listed in your requirements.txt file
for any updates and can update them via automatically generated pull requests. This helps maintain your repo from 
security issues and stay on the latest versions of your dependencies.

### How to Set Up Dependabot

See the [Dependabot quickstart guide](https://docs.github.com/en/code-security/getting-started/dependabot-quickstart-guide)
for more info.

1. Navigate to the GitHub repository you add Dependabot to.
2. Go to the Insights tab > Dependency graph > Dependabot tab. *** You can also do this through Settings > Code Security 
and analysis > Dependabot. This option will allow more granularity on what kinds of alerts you want to include.
3. Click the "Enable Dependabot" button as seen below. This will automatically create a .github folder in your 
repository and a dependabot.yml file within that folder.

![enable_dependabot_github_procedures](https://github.com/uga-libraries/GitHub_Standards/assets/62658840/038e82a2-283c-4929-b020-945d24c1d3aa)

4. You'll be taken to the dependabot.yml file where you can fill out the appropriate settings
(see [Configuration Options for Dependency Updates](https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates)
for more info). The settings we typically use include:
   1. package-ecosystem: "pip"
   2. directory: "/" - if you have a requirements.txt file at the top level of your repo, it should grab that
   3. schedule: interval: "weekly"

![dependabot_file_settings](https://github.com/uga-libraries/GitHub_Standards/assets/62658840/8ee88d8a-47e5-481e-81a4-9c6f61a84c3e)

5. Commit changes in the top right corner to save your settings.
6. You should now receive dependabot pull requests to update your dependencies.

### Accepting Pull Requests

See [About pull request merges](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/about-pull-request-merges)
for more info.

If enabled, Dependabot will automatically generate pull requests to update any dependencies once a new version is 
released. To merge these pull requests, use the following:

1. Navigate to the Pull requests tab at the top left of your repository's GitHub page.
2. Select the pull request you want to merge.

![select_pull_request_dependabot](https://github.com/uga-libraries/GitHub_Standards/assets/62658840/af12a008-de75-4bad-a399-814776012a0b)

3. Review the pull request to make sure you want to make this change. You can select the Files changed tab to see what
the pull request will change as part of your code.

![pull_request_description_dependabot](https://github.com/uga-libraries/GitHub_Standards/assets/62658840/f4b48c70-92a6-4d2d-9c57-b893fe24cb2e)

4. Click "Merge pull request" or select one of 3 options in the green drop down box (recommend Squash and merge).
   1. Create a merge commit - all commits will be added from this pull request and changes merged into your base (main)
   branch.
   2. Squash and merge (recommended) - condense all commits into one commit and merge the changes into your base (main) 
   branch.
   3. Rebase and merge - all commits from the pull request are added to the base (main) branch individually
      (see [Rebase and merge your commits](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/about-pull-request-merges#rebase-and-merge-your-commits)).

![merge_options_dependabot](https://github.com/uga-libraries/GitHub_Standards/assets/62658840/c4010240-0a63-4501-80dc-a493f69c55fe)

5. After selecting your commit and merge option, the requirements.txt file should be updated with the new pull request 
on your base (main) branch and commit(s) added to your commit history.