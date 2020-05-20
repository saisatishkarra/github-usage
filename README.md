# github-usage
Demo the github-usage workflows

### Worflow mainly categories on two concepts:
1. Does production involve multiple versions for each customer?
2. Does production have single version and every other release is based of single version?

### Dataguise SaaS Use-Case
1. We have a SaaS product with multiple versions for use in production for different customers and we would pick **gitflow** VS **one-flow** , **gitlab-flow**, **github-flow** , **gitflow**

### Git flow:
1. master — this branch contains production code. All development code is merged into master in sometime.
2. develop — this branch contains pre-production code. When the features are finished then they are merged into develop.
During the development cycle, a variety of supporting branches are used:
3. feature-* — feature branches are used to develop new features for the upcoming releases. May branch off from develop and must merge into develop.
4. hotfix-* — hotfix branches are necessary to act immediately upon an undesired status of master. May branch off from master and must merge into master anddevelop.
5. release-* — release branches support preparation of a new production release. They allow many minor bug to be fixed and preparation of meta-data for a release. May branch off from develop and must merge into master anddevelop.

Advantages:

Ensures a clean state of branches at any given moment in the life cycle of project
The branches naming follows a systematic pattern making it easier to comprehend
It has extensions and support on most used git tools
It is ideal when there it needs to be multiple version in production

Disadvantages:

The Git history becomes unreadable
The master/develop split is considered redundant and makes the Continuous Delivery and the Continuos Integration harder
It isn’t recommended when it need to maintain single version in production
