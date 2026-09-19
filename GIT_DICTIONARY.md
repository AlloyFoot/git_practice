# GIT DICTIONARY

## SETUP
- git init
\ncreates an empty Git repo
- git config
\nused to get and set config variables that control how Git looks, behaves, and operates.

## MAKING COMMITS
- git add
\nmoves changes from working directory to Git staging area
- git add -u
\ndoes "git add" but for the entire repo - NOT NEW FILES
- git add .
\ndoes "git add" but for the entire repo - INCLIDING NEW FILES
- git commit
\ncaptures a snapshot of project's currently stages changes to local repo
uses Vim/default test editor to create message
- git commit -m "..."
does "git commit" but doesn't open Vim for the message

## BRANCHES
- git switch
switches branches
- git switch -c
creates and switches branches
- git branch
prints all branches to Terminal 
OR
creates new branch
- git branch -d
deletes a branch (pushed, will not delete an "unsaved" branch)
- git branch -D
deletes a branch (all)

## REMOTES
- git remote
used to create, view, and delete connections between your local repository and remote repos
- git remote set-url
changes the URL string associated with an existing remote nickname
- git push
uploads local repo to a remote repo
- git pull
downloads changes from a remote repo and integrates them into your local branch
- git fetch
downloads commits, files, and reference from a remote repo to your local machine
does not merge or integrade into your active working files
Run git status to see how many commits your local branch is behind the remote version.
Use git diff main origin/main to view the exact code changes line-by-line before accepting them.
If you like what you see and are ready to update your files, you can manually run git merge origin/main to safely merge the changes.
- git fetch --prune
removes local references to remote branches that no longer exist

## PULL REQUESTS
- gh pr create
creates a pull request on GitHub
- gh pr status
displays a real-time summary of all relevant pull requests for your current repository
- gh pr merge
merge a GitHub pull request

## USEFUL GITHUB CLI 
- gh auth login
authenticates your terminal with your GitHub account
- gh auth status
displays your active account and tests the current authentication state across all known GitHub hosts
