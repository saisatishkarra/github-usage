# github-usage
Demo the github-usage workflows

### Worflow mainly categories on two concepts:
1. Does production involve multiple versions for each customer?
2. Does production have single version and every other release is based of single version?

### Dataguise SaaS Use-Case
1. We have a SaaS product with multiple versions for use in production for different customers and we would pick **gitflow** VS **one-flow** , **gitlab-flow**, **github-flow** , **gitflow**

### One Flow

### Get-To-Know:
1. Master is the mainstream branch for production directly or via use of tags/releases.
2. Naming conventions should be either feature/<name_of_feature> , bugfix/<bug_fix_description>, hotfix/<hotfix_description>, release/<version-number>
3. Bug Fixes are considered as features
4. Releases can be code freezes, producing Release Candidates, and having a full QA process that branch off from master using tags and doesn't always start from tip of master. Starts from a stable version within master.

    ```
    git checkout development

    git checkout -b release/2.3.0 <stable-commit-hash>
    ```
5. Hotfix branches are cut from the commit that the latest release version tag points to.    
    ```

    ```