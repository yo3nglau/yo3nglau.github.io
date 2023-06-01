---
title: git add
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
git-add - Add file contents to the index
```

## Description

This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit.

The "index"  holds a snapshot of the content of the working tree, and it is this snapshot that is taken as the contents of the next commit.

Thus after making any changes to the working tree, and before running the commit command, you must use the `add` command to add any new or modified files to the index.

The [`git status`](https://git-scm.com/docs/git-status) command can be used to obtain a summary of which files have changes that are staged for the next commit.

## Options

**`<pathspec>…`**

​	Files to add content from.

**`-f, --force`**

​	Allow adding otherwise ignored files.

**`-A, --all, --no-ignore-removal`**

​	Update the index not only where the working tree has a file matching `<pathspec>` but also where the index already has an entry. This adds, modifies, and removes index entries to match the working tree.

## Resources

https://git-scm.com/docs/git-add

https://git-scm.com/docs/git-status