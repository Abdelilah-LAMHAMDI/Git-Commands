# Git Console Commands Cheat Sheet

This document is a complete, faithful English translation of the original Russian Git cheat sheet.

## General
Git is a version control system (VCS) for files. It is similar to saving in computer games (a commit is like a save).

Important: adding files to a commit is a two-step process:
1. Add files to the index (git add)
2. Save changes (git commit)

Tracked files can be unchanged, modified, or staged.

## Key Concepts – Three Trees
- Working directory
- Index (staging area)
- .git directory

## Commits
A commit is an immutable snapshot of changes.

## Basic Workflow
Edit → Add → Commit → Repeat

## Configuration
```
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
```

Windows:
```
git config --global core.autocrlf true
```

## Copying Commits (Cherry-pick)
```
git cherry-pick 5589877
git cherry-pick master~2..master
git cherry-pick -n 5589877
git cherry-pick master..feature
git cherry-pick --abort
git cherry-pick --continue
```

## Branches
```
git branch
git checkout -b new-branch
git merge feature
```

## Remotes
```
git remote add origin URL
git fetch origin
git pull origin master
git push origin master
```

## Archive
```
git archive -o project.zip HEAD
```

## .gitattributes
```
* text=auto
*.html diff=html
*.css diff=css
*.scss diff=css
```
