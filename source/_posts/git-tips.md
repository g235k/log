---
title: Git Tips
date: 2021-03-14 17:11:57
categories: Tech
tags:
  - Git
  - Version Control
---

## Config

```
git config --global user.email "aleph@infty.null" 
git config --global user.name "aleph"
```

or remove `--global` to config under a certain repo

```
git config --list
```

## Commit

```
git remote add origin git@github.com:aleph/learning.git
git add .
git commit -m "https://hexo.io/docs/github-pages.html"
```
[Using the option `-am`](https://stackoverflow.com/questions/19877818/git-commit-m-vs-git-commit-am/19877909) allows you to **add** and **create a message for the commit** in one command.

Some of your files are not staged. This occurs with deleted/added files that are not currently being tracked. Usually, you have to do a `git add -u` in order to stage "untracked" files. `-am` will do this for you as well.

you might be looking for `git add -A` which is the same as `git add --all`, which is different than `git add .`

```
git status
```

## Push

```
git push -u origin master
```

[The `-u` option automatically sets the upstream for you]((https://stackoverflow.com/questions/5561295/what-does-git-push-u-mean)), so you can use `git pull` or `git push` **without arguments**.

It's worth pointing out that the branch which is pushed to with `git push` [isn't affected by the upstream branch configuration](https://longair.net/blog/2011/02/27/an-asymmetry-between-git-pull-and-git-push/) unless you have `push.default` set to `tracking` (or `upstream` in later versions of git).
