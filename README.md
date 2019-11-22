# Git 101

[Git](https://git-scm.com/) is a distributed version-control system, created by [Linus Tolvalds](https://en.wikipedia.org/wiki/Linus_Torvalds) in 2005. Git is practical, simplified, fast, efficient, and free and open source. 

## First commands

| Name     	| Command                                              	| Description                                     	|
|----------	|------------------------------------------------------	|-------------------------------------------------	|
| Init     	| `git init`                                           	| Create directory configured as a git repository 	|
| Status   	| `git status`                                         	| Show repository status                          	|
| Add      	| `git add <file name>`                                	| Add new and modified files for next commit      	|
| Commit   	| `git commit -m 'description'`                        	| Register commit with all files you used git add 	|
| Log      	| `git log`                                            	| View latest commits in repository               	|
| Settings 	| `git config --global user.email "you@example.com ”` 	| Set up your email (only the first time)            	|
|          	| `git config --global user.name “Your Name”`          	| Set up your name (only the first time)              	|

#### File status

* :x: Untracked 
* :new: Modified 
* :ok: Staged 
* :heavy\_check\_mark: Committed

#### Workflow 

* :scissors: **Edit**,
* :memo: **Commit**, and 
* :arrows\_clockwise: **Sync** with remote repository

## Create a remote repository

| Name   	| Command                        	| Description                                	|
|--------	|--------------------------------	|--------------------------------------------	|
| Remote 	| `git remote -v`                	| Configure the server                       	|
|        	| `git remote add <remote><url>` 	| Add another remote server                  	|
| Push   	| `git push -u origin master`    	| Sync with remote repository the first time 	|
|        	| `git push`                     	| Sync with remote repository                	|
| Clone    	| `git clone <url>`             	| Download remote repository                                  	|
| Pull     	| `git pull`                    	| Keep repository synchronized with last branch commits       	|


## History and conflicts

| Name     	| Command                       	| Description                                                 	|
|----------	|-------------------------------	|-------------------------------------------------------------	|
| Diff        	| `git diff [path]` 	| Display differences between commits and branchs           	|
|             	| `git diff HEAD~1` 	| Shows what was changed in the last commit                 	|
| Checkout 	| `git checkout <commit><file>` 	| Shows how a file or entire repository was in a given commit 	|
|          	| `git checkout <commit>`       	| Changes the repository to that commit state                 	|
|          	| `git checkout master`         	| To return the repository at last commit                     	|
|        	| `git checkout -- <path_or_file>`   	| Undo all non-stage changes since the last commit                   	|
|        	| `git checkout HEAD -- <path_file>` 	| Undo changes since last commit including stage                     	|
| Revert 	| `git revert <commit>`              	| Creates a new commit that undoes changes to the specified commit   	|
| Reset  	| `git reset <commit>`               	| Reset repository for a given commit                                	|
|        	| `git reset --hard <commit>`        	| Resets and removes all changes :exclamation: Be careful when using 	|

## Branch, Merge and Rebase

| Name   	| Command                   	| Description                                                                                                                                                                                                                                                                                             	|
|--------	|---------------------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Branch 	|                           	| Branch master is the default. Development branch make it easy to control                                                                                                                                                                                                                                	|
|        	| `git branch <new_branch>` 	| Create a new branch                                                                                                                                                                                                                                                                                     	|
|        	| `git branch -d <branch>`  	| Delete a branch                                                                                                                                                                                                                                                                                         	|
|        	| `git checkout <branch>`   	| Switch to the branch                                                                                                                                                                                                                                                                                    	|
| Merge  	| `git merge <branch>`      	| Commit a branch to the current branch. Finds a common commit (base) between branches and applies all commits that the current branch doesn't have. If there are commits in the current branch that is not in the other branch, a merge commit will be created.                                          	|
| Rebase 	| `git rebase <branch>`     	| Similar to Merge but different in the order of committing. In Rebase, your commits in front of the base are temporarily removed, commits from another branch are applied to your branch, and finally your commits are applied one by one. There may be conflicts that will be resolved for each commit. 	|
| Fetch  	| `git fetch`               	| pull = fetch + merge. Download remote updates but do not apply them to the repository. Lets you rebase a branch instead of merge. Fetch and rebase is best for keeping track of development.                                                                                                            	|
| Tag    	| `git tag [name_tag]`      	| Useful for defining stable versions of the project                                                                                                                                                                                                                                                      	|

## Other commands

| Name        	| Command                   	| Description                                                                                                                                                                      	|
|-------------	|---------------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Amend       	| `git commit --amend`      	| Changes the last commit                                                                                                                                                          	|
| Stash       	| `git stash`               	| Save Working Directory Changes. Allows you to rebase, merge, switch branches without the need to commit.                                                                         	|
|             	| `git stash list`          	| Applies the last stored stash.                                                                                                                                                   	|
|             	| `git stash pop`           	|                                                                                                                                                                                  	|
| Cherry Pick 	| `git cherrypick <commit>` 	| Applies commit changes to the current branch. Create a new commit. Useful to retrieve history                                                                                    	|
| Blame       	| `git blame`               	| Shows changes made to one file per line. Show author and commit that line was made. Useful to check when changes were made, why, and by whom                                     	|
| Bisect      	| `git bisect`              	| Lets you do a binary search in commits to find a change. Useful for changes that have changed behavior and cannot be easily identified by code. When the change may be quite old 	|


---

## References

* [https://git-scm.com/](https://git-scm.com/)
* [https://brorlandi.github.io/curso-git/](https://brorlandi.github.io/curso-git/)
* [https://www.udemy.com/course/git-e-github](https://www.udemy.com/course/git-e-github)


