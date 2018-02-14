## Why Contribute?

Keeping the information and advice in PMRoK up to date is important not only
for the Voyage that's currently in progress, but also for future Voyages.
Not only does contributing help build the repository of PM knowledge for the
PM's that will follow you, but doing so will also help you to improve and
extend your PM skills.

## How to Contribute

Making corrections or adding content to PMRoK follows a process very
similar to the one you use when making contributions to your Voyage projects. 
GitHub Wiki's are implemented in a manner that doesn't allow changes to be
approved and merged using the Pull Request (PR) mechanism available to normal
repos.

Due to this, a "mirror" repo has been created that you will use to make changes
just like you do in a normal project repo. TravisCI integration has been set
up in the mirror to automatically push changes from the `master` branch once
a PR for a change has been reviewed, approved, and merged from `development`
into `master`.

This architecture was adapted from this [article](http://www.growingwiththeweb.com/2016/07/enabling-pull-requests-on-github-wikis.html)
and the following diagram depicts the change management flow for PMRoK.

![PMRoK Change Management Workflow](https://github.com/Chingu-cohorts/pmrok/blob/development/diagrams/PMRoK%20Change%20Mgt%20Workflow.png)

1. Start by cloning the "mirror" repo, [pmrok-chgmgt](https://github.com/Chingu-cohorts/pmrok-chgmgt),
your computer. By default the `development` branch will be cloned onto your computer.
2. Create a new _working branch_ with a descriptive name. For example, `fix/softskill-url`.
Any changes or additions to make should be made to this working branch. Remember to issue frequent commits if you are making multiple changes so there is a detailed trail of each change you've made.
3. When you are ready to share with others or if you just need to ensure that your in progress work
is backed up, push your changes to the `pmrok-chgmt` repo using the same working branch name. For
example, `git push origin fix/softskill-url`.
4. If you should need to refresh your working branch from GitHub simply
`git pull origin <working-branch>`.
5. When your changes are completed you can start the process of promoting them to the wiki by
creating a PR to merge your changes into the `development` branch. Be sure to select `PMCAB` as
the reviewer and once changes have been reviewed and approved, you will be responsible for 
performing the merge.
6. Once your change has been merged into the `development` branch it will be ready to merge into
the `master` branch along with changes submitted by others. A member of the _PMRoK Change Approval
Board (PMCAB)_ will periodically create a PR to promote all changes from `development` to `master`.
7. Merging into `master` by a member of the PMCAB will automatically start the TravisCI integration
script to move changes to the PMRoK Wiki.
8. Once the TravisCI integration script has completed the approved changes will be available to
all users of the PMRoK Wiki.

If you are curious about the _Change Approval Board_ process it is a concept that's part of the
[Information Technology Infrastructure Library](https://en.wikipedia.org/wiki/ITIL), which is a
set of best practices for managing IT infrastructure assets. 
