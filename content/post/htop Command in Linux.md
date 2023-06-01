---
title: htop Command in Linux
author: yo3nglau
date: '2023-05-26'
categories:
  - Technical Blogs
tags:
  - Linux Commands
---

## Name

```
htop - interactive process viewer
```


## Syntax

```
htop [-dChustv]
```

## Description

htop command in Linux system is a command line utility that allows the user to interactively monitor the system’s vital resources or server’s processes in real time. htop is a newer program compared to top command, and it offers many improvements over top command. htop supports mouse operation, uses color in its output and gives visual indications about processor, memory and swap usage. htop also prints full command lines for processes and allows one to scroll both vertically and horizontally for processes and command lines respectively.

## Options

```
-d --delay=DELAY
      Delay between updates, in tenths of seconds

-C --no-color --no-colour
      Start htop in monochrome mode

-h --help
      Display a help message and exit

-p --pid=PID,PID...
      Show only the given PIDs

-s --sort-key COLUMN
      Sort by this column (use --sort-key help for a column list)

-u --user=USERNAME
      Show only the processes of a given user

-v --version
      Output version information and exit

-t --tree
      Show processes in tree view
```

## Resources

https://manpages.ubuntu.com/manpages/focal/en/man1/htop.1.html