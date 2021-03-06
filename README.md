# git-my

Lists all of a user's branches, including local and remote, and shows:

- if a remote branch is checked out locally
- if a local branch is tracked remotely
- if a local branch is up-to-date with a specified branch

| Name          | Link     |
| ------------- | -------- |
| Project Home: | [https://github.com/davidosomething/git-my](https://github.com/davidosomething/git-my)

## About

Unlike `git branch -r` and `git remote show origin` this shows only branches
where YOU were the last committer and it will tell you if you have a copy of
that branch locally.

Here's a screenshot:  
![Example output](https://raw.githubusercontent.com/davidosomething/git-my/docs/screenshot.png)

## Installation

- Requires BASH 4+
- Add the `git-my` file somewhere in your path, e.g. `/usr/local/bin/`

### zplug installation

Super simple if you use zplug:

```sh
zplug "davidosomething/git-my",   as:command
```

## Usage

From command line execute:

    git my

### Options

#### Remote comparison branch

    git my origin/qa

will give you a list of your remote branches and tell you which ones have been
merged into `origin/qa`.

## To do

    -v|--version
    -h|--help
    -U|--username
    --local
    --merged
    --tracked


----

Copyright (c) 2017 David O'Trakoun <me@davidosomething.com>

