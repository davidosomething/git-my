# git-my v1.0.0

Lists all of a user's branches, including local and remote, and shows:

- if a remote branch is checked out locally
- if a local branch is tracked remotely
- if a local branch is up-to-date with a specified branch

| Name | Link |
| ---- | ---- |
| Project Home: | [https://github.com/davidosomething/git-my](https://github.com/davidosomething/git-my)

## About

Unlike `git branch -r` and `git remote show origin` this shows only branches
where YOU were the last committer and it will tell you if you have a copy of
that branch locally.

Here's a screenshot:
![Example output](https://raw.githubusercontent.com/davidosomething/git-my/docs/screenshot.png)

## Installation

- Add the `git-my` file somewhere in your path, e.g. `/usr/local/bin/`

## Usage

From command line execute:

```
git my
```

### Options

Currently git-my supports one argument, the remote branch to test against. E.g.
running:

```
git my origin/qa
```

will give you a list of your remote branches and tell you which ones have been
merged into `origin/qa`.

## To do

- Options support

```
  -v|--version
  -h|--help
  -d|--decorate       LOCAL,MERGED
  -r|--remote-ref     origin/master
  -U|--username
  --no-color
  --no-header
  --no-decorate
```

----

Copyright (c) 2015 David O'Trakoun <me@davidosomething.com>

