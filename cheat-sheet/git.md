---
title: Git Cheat Sheet
author: Danny Cheung
tags:
  - git
  - cheat sheet
---

| Command | Description |
| ------- | ----------- |
| ```git rev-parse --abbrev-ref HEAD``` | Get current branch name |
| ```git branch -d "${BRANCH}"``` | Delete local copy of a branch |
| ```git push origin :"${BRANCH}"``` | Delete remote copy of a branch |
| ```git stash save "${STASH_MSG}"``` | Save uncommitted changes to `git stash` with a message |
| ```git stash list \| grep "${STASH_MSG}" \| cut -d: -f1``` | Get the name of the git stash entry correcsponding with the stash message |
| ```git stash pop "${STASH_NAME}"``` | Apply uncommitted changes stored in git stash |
| ```git merge "${SOURCE_BRANCH}"``` | Pull in commits from another branch |
