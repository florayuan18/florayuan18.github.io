---
layout: page
title: GitHub Guide
subtitle: Flora Yuan
---
## Purpose
- To organize pull requests and commits
- To prevent commit errors and loss of code
- To organize and efficiently delegate tasks
- To avoid committing files that don’t belong in version control

## GitHub Project Setup
- ReadMe to organize journals, commits, profiles, and individual issues
- ReadMe must be frequently updated by all team members
- Inclusion of a .gitignore file to ensure that files not tracked by Git remain untracked
- Additional lines may be added into the .gitignore file to tell GitHub to ignore them, with the consensus of group members
- .idea files:

## Scrum Board
- Split up into different sections to track progress (To Do, In Progress, Teacher Review Ready, and Done columns)
- Individual issues that are assigned and labeled appropriately at the beginning of the week
- Individual issues must be moved to the Done column and closed once completed
- Tasks must be completed in the week assigned unless deadlines are extended
- Members must look 3 weeks ahead to plan accordingly

## Pull Requests
- Members will try not force pushes by and instead discuss with others in the team to problem solve
- Topic branches will be used for pull requests
- Team members will tell one another when they have pushed to the topic branch
- Team members will pull changes by the end of each class period
- For larger technicals, pull requests will be drafted and created
- Members can push commits from the topic branch and add them to the pull request
- Other members will review proposed changes, add review comments, and possibly add their own commits to the pull request

## Branches Techniques
- Individual technicals will be conducted on separate branches
- Git-checkout will be used to update individual branches
- Only merge after checking with other members to prevent merging errors
- Rebasing can be for the entire branch or just a single commit

## How to Create and Merge a Branch
- Merging to master the most common way to integrate results of work back into the main code base
- Integrated into the head of the target branch
- Click checkout to switch to a branch (under Git)
- Branches popup - Branches
- Rebasing branches (git-rebase)
- Rebasing from one branch to the other
- Rebase operation integrates changes on feature branch to master branch by applying commits on top of current HEAD commit in master
- Git | Rebase - choose target branch to which you want to rebase to
- Can do rebasing from a particular commit instead of entire branch
- Modify options and choose --onto
- Enter the hash of the commit

## Forks
- No forks (independent of the original repository) will be used


# Week 3
## Commits
- Calvin: He worked on getting the new FRQs to work on his page, specifically creating a .java file for the order [FRQ](https://github.com/florayuan18/pikachudrinkingwindex/commit/8821ca1cd2fa2ad6357a82fce79db91de9cf3494).  He also made progress with the [API](https://github.com/florayuan18/pikachudrinkingwindex/commit/5ba5543753fe4c135bbb929050a6ea974dfb3990#diff-5452d644105363cac4fbcb3928edf554a575b4312c9898f78c357c2ca531f1d0R1-R45).
- Kira: She worked on updating her "about us" page with the FRQs as well, finalizing the controller for the light [sequence](https://github.com/florayuan18/pikachudrinkingwindex/commit/b32a4428b2534f39171615c5ce9dc589ce7a9673).  She also made progress with [designing](https://github.com/florayuan18/pikachudrinkingwindex/commit/11003c2f3ec97c38f9ed0b3d34ff3600563838b0#diff-dce5037ca59f91a501819f7f56f1c6c1425519e96cb2fdde9c7dbce971c179e9R5-R62) the website.
- Maggie: She worked on the FRQs as well, creating a controller for the order [FRQ](https://github.com/florayuan18/pikachudrinkingwindex/commit/0f9bb6a6d7d93a4750cca432f8bb39ba5d595a1c)
- Flora: She worked on the FRQs, as well as started updating the navigation bar to start creating a [theme](https://github.com/florayuan18/pikachudrinkingwindex/commit/30d3a2cfb5b0172359bce0e3131df9418f3e77e0).
- Crystal: She updated the readme to include the timebox for week 3 [material](https://github.com/florayuan18/pikachudrinkingwindex/commit/c5e518ee63ac61da98283e6d2029fcb538b077c8)

## Pull Requests
- Pull Request created for the design branch for implementing CSS into the main [branch](https://github.com/florayuan18/pikachudrinkingwindex/pull/43)