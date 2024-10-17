---
date: 2024-10-17
tags:
  -  #fact
hubs:
  - "[[git]]"
urls: https://stackoverflow.com/a/44036640
  -
---

# Conditional includes git

Since git 2.13 it is possible to have multiple user/email coexist on single machine.

```
# ~/.gitconfig
...
settings
...
[include]
    path = .gitconfig-work
[includeIf "gitdir/i:/personal/"]
    path = .gitconfig-personal
```
