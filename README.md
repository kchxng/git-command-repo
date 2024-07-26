![all text](git_logo.jpg)

# Git command there we always use to manage the project

Keeping the git command line that we usually use to manage coding

- Reffer Documentation [Click Here](https://www.w3schools.com/git)

## List the git versions

```bash
git --version
```

## Init git configuration

```bash
git init
```

## See the git status

```bash
git status
```

## Git Add

```bash
git add ex1.ts ex2.ts # Add single file
# or
git add . # Add all files
```

## Hold files, but need to reuse it on the feature (No commit changes)

- Use git stash to hidden files there are not complete yet, But need to switch to another branch

```bash
git add ex1.ts # Add before hidden
git stash
git stash list # List files that were hidden
git stash pop # Reuse the files that were stash or hidden
#
```

## git commit

```bash
git commit -m "<description of comments>"
```

## Push directory to git repository

```bash
git push origin <branch-name>
git push # Only main branch
# or force
git push origin <branch-name> --force
```

## Pull coding from git repository

```bash
git pull origin <branch-name>
git pull # Only main branch
```

## Clean repository when pulling

```bash
git pull origin <branch_name> --prune
```

## Create a new branch

```bash
git branch <branch-name>
# or
git branch switch -c <branch_name> # Create new branch and switch to
# or
git checkout -b <branch_name>
```

## Rename a branch

```bash
git branch -m <old_branch> <new_branch>
# ex:
git branch -m branch-a branch-b
```

## Switch to a new branch

```bash
git switch <branch_name>
# or
git checkout <branch_name>
```

## Merege branch

```bash
git merge <branch_a>
# ex: Need to merge branch-a into branch-b
git switch branch-a
git merge branch-b
```

## Delete a branch

```bash
git branch -d <branch_name>
# or
git branch -D <branch_name>
```

## Refresh when a branch is updated

```bash
git fetch
```

## Cleanup or Refresh branches when were we delete on git server

```bash
git fetch --all --prune
```

## Tags version

```bash
git tag <version>
# ex:
git tag v1.0.0
```

## Git Rollback and cleanup squashed

```bash
git reset --hard <squash_code>
# ex:
git reset --hard ce34ds
```

## Add Origin URL to repository

```bash
git remote add origin <git-url>
```

## Remove URL from local repository

```bash
git remote remove origin
```

## When .gitignore is not working that way to resolve

```bash
git reflogprune
git prune
```

## Monitor repository log

```bash
git log # monitoring log only
git log --oneline # monitoring log with one line
git log --oneline --graph # monitoring log with one line and graph
git log --oneline --graph --all # monitoring log with one line and all graph
```
