# hackattoni

This repository aims to create a script that enhance automation of the workflow for creating PR on github.



## Goals

- Automate creation of PR targeting master
- Automate creation of PR targeting stable branches

### Automate creation of PR targeting master

We can ease this step by creating a script that does the following:
- [x] Create PR on master
  - [ ] the body of the PR should be pre-compiled before as much as possible
  - [ ] the custom parts are:
    - [ ] description
    - [ ] new behaviour
- [x] Assign PR to yourself
- [x] Copy from issue: 
  - [x] labels
  - [x] milestone
- [ ] Connect PR to issue (zenhub API)


### - Automate creation of PR targeting stable branches

The steps here are the same as if the PR is made on master but a few extra are needed:

- [ ] add label backport
- [ ] add reviewer from original PR
- [ ] title of PR should be: Backport STABLE_BRANCH - (#ISSUE_NUMBER) PR_TITLE (#PR_NUMBER)
- [ ] body of PR should be:
  - [ ] # Description
  - [ ] Copy title of this backport PR
  