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


## Create a remote repository

| Name   	| Command                        	| Description                                	|
|--------	|--------------------------------	|--------------------------------------------	|
| Remote 	| `git remote -v`                	| Configure the server                       	|
|        	| `git remote add <remote><url>` 	| Add another remote server                  	|
| Push   	| `git push -u origin master`    	| Sync with remote repository the first time 	|
|        	| `git push`                     	| Sync with remote repository                	|

## File status

| Name        	| Command           	| Description                                               	|
|-------------	|-------------------	|-----------------------------------------------------------	|
| Workflow    	|                   	| **Edit**, **Commit**, and **Sync** with remote repository 	|
| File Status 	|                   	| Untracked / Modified / Staged / Committed               	|
| Diff        	| `git diff [path]` 	| Display differences between commits and branchs           	|
|             	| `git diff HEAD~1` 	| Shows what was changed in the last commit                 	|




---

## References

* [https://git-scm.com/](https://git-scm.com/)
* [https://brorlandi.github.io/curso-git/](https://brorlandi.github.io/curso-git/)
* [https://www.udemy.com/course/git-e-github](https://www.udemy.com/course/git-e-github)


