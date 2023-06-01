---
title: git commit
author: yo3nglau
date: '2023-05-22'
categories:
  - Technical Blogs
tags:
  - Git Commands
toc: true
---

## Name

```
git-commit - Record changes to the repository
```

## Description

Create a new commit containing the current contents of the index and the given log message describing the changes. The new commit is a direct child of HEAD, usually the tip of the current branch, and the branch is updated to point to it.

The content to be committed can be specified in several ways:

1. by using [git-add](https://git-scm.com/docs/git-add) to incrementally "add" changes to the index before using the *commit* command (Note: even modified files must be "added");
2. ...

## Options

**`-a, --all`**

​	Tell the command to automatically stage files that have been modified and deleted, but new files you have not told Git about are not affected.

**`-m <msg>, --message=<msg>`**

​	Use the given `<msg>` as the commit message. If multiple `-m` options are given, their values are concatenated as separate paragraphs.

## Resources

https://git-scm.com/docs/git-status

https://git-scm.com/docs/git-add