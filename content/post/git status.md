---
title: git status
author: yo3nglau
date: '2023-05-22'
categories:
  - Technical Blogs
tags:
  - Git Commands
toc: true
---

## Name

*git-status - Show the working tree status*

## Description

Displays paths that have differences between the **index file** and the **current HEAD commit**, paths that have differences between the **working tree** and the **index file**, and paths in the working tree that are not tracked by Git. The first are what you *would* commit by running `git commit`; the second and third are what you *could* commit by running `git add` before running `git commit`.

## Options

**`-s, --short`**

​	Give the output in the short-format.

**`--long`**

​	Give the output in the long-format. This is the default.

### Short Format

In the short-format, the status of each path is shown as one of these forms

```
XY PATH
XY ORIG_PATH -> PATH
```

where `ORIG_PATH` is where the renamed/copied contents came from. `ORIG_PATH` is only shown when the entry is renamed or copied. The `XY` is a two-letter status code.

There are three different types of states that are shown using this format, and each one uses the `XY` syntax differently:

- When a merge is occurring and the merge was successful, or outside of a merge situation, `X` shows the status of the index and `Y` shows the status of the working tree.
- When a merge conflict has occurred and has not yet been resolved, `X` and `Y` show the state introduced by each head of the merge, relative to the common ancestor. These paths are said to be *unmerged*.
- When a path is untracked, `X` and `Y` are always the same, since they are unknown to the index. `??` is used for untracked paths. Ignored files are not listed unless `--ignored` is used; if it is, ignored files are indicated by `!!`.

Note that the term *merge* here also includes rebases using the default `--merge` strategy, cherry-picks, and anything else using the merge machinery.

In the following table, these three classes are shown in separate sections, and these characters are used for `X` and `Y` fields for the first two sections that show tracked paths:

- ' ' = unmodified
- *M* = modified
- *T* = file type changed
- *A* = added
- *D* = deleted
- *R* = renamed
- *C* = copied
- *U* = updated but unmerged

## Resources

https://git-scm.com/docs/git-status