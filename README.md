# 50 Git questions (with answers)

A list of 50 frequently git questions with answers.
Released under a [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.

**WARNING**: not yet finished...


#### 1. How to check if git is available on your system?

``` bash
$ git --version
```



#### 2. How to initialize a new Git repository?

``` bash
$ git init project
$ cd project
```



#### 3. How to tell git about your name and email?

``` bash
$ git config --global user.name "<your name>"
$ git config --global user.email "<your email>"
```



#### 4. How to tell git to not use vi as the default editor?

``` bash
$ git config --global core.editor "nano -w"
```



#### 5. What is the staging area?

The staging area is an intermediate storage for changes that will be part of the
next commit.



#### 6. How to add a file to the staging area?

``` bash
$ git add <file>
```



#### 7. How to remove a file from the staging area?

``` bash
$ git reset HEAD -- <file>
```



#### 8. How to make a commit?

``` bash
$ git commit -m "Commit message"
```

#### 9. Where are git preferences saved?

``` bash
$ git config --list --show-origin
```

#### 10. How to ignore untracked files?

Add them to a local `.gitignore` file

#### 11. How to untrack a file without deleting it?

``` bash
$ git rm --cached <file>
```

#### 12. How to undo the most recent commit?

``` bash
$ git reset HEAD~
$ nano <file>
$ git add <file>
$ git commit -c ORIG_HEAD
```

#### 13. How to change the message of the last commit?

``` bash
$ git commit --amend -m "New message"
```

#### 14. How to add a remote repository?

``` bash
$ git remote add <name> <url>
```

#### 15. How to compare a file to the last committed version?

``` bash
$ git diff HEAD -- <file>
```


#### 16. How to rename a remote?

``` bash
$ git remote rename <old_name> <new_name>
```

#### 17. How to change the address of a remote?

``` bash
$ git remote set-url <name> <new_url>
```

#### 18. How to send your changes to a remote repository?

``` bash
$ git push
```


#### 19. How to synchronize your local and remote repositories?
#### 20. What is the different between `reset` and `revert`?
#### 21. How to tell git to ignore trailing whitespaces?
#### 22. What is the difference between `git add *; git commit` and `git commit -a -m`?
#### 23. What is the difference between `pull` and `fetch`?
#### 24. How to make a commit from another author?

```bash
$ git commit --author "Name Surname <email@address>" ...
```

#### 25. How to create a branch?
#### 26. How to switch to a branch?
#### 27. How to know when a file was first added to the repository?
#### 28. How to get a list of all deleted files?
#### 29. How to completely remove (sensitive) files from history?
#### 30. How to list remote repositories?

```bash
$ git remote -v
```

#### 31. How to tag a specific commit?

```bash
$ git tag -m '...' <commit>
```

#### 32. How to get a list of tags?

```bash
$ git tag
```

#### 33. How to merge 3 last commits into a single one?
#### 34. How to get last modification for a given file?
#### 35. How to swap branch master with another one?
#### 36. How to access all commits in case of problem?
#### 37. How to get all the commits from a specific user?
#### 38. How to ignore the .gitignore file?
#### 39. How to get the list of unpushed commits?

```bash
$ git log @{u}..
```

#### 40. How to compare a file across two different branches?

```bash
$ git diff <branch-a> <branch-b> -- <file>
```

#### 41. How to merge two git repositories?
#### 42. What is the difference between HEAD and ORIG_HEAD?
#### 43. How to use a global .gitignore?

Create `~/.config/git/ignore` with a list of patterns.

#### 44. What if the difference between `rm` and `git rm`?
#### 45. How prevent a push if remote has extra commits?

This is the default with `git push`, not necessary to do anything.

#### 46. How to create a git alias command?
#### 47. How to undo a pushed commit?
#### 48. How to find the first commit?
#### 49. How to find top contributor?
#### 50. 
